# Comparing `tmp/cf-view-3.1.0.tar.gz` & `tmp/cf-view-3.2.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf-view-3.1.0.tar", last modified: Mon Mar  6 17:06:27 2023, max compression
+gzip compressed data, was "cf-view-3.2.22.tar", last modified: Thu May 18 10:12:50 2023, max compression
```

## Comparing `cf-view-3.1.0.tar` & `cf-view-3.2.22.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-03-06 17:06:27.009531 cf-view-3.1.0/
--rw-r--r--   0 andy      (1000) andy      (1000)     1065 2021-06-09 09:47:44.000000 cf-view-3.1.0/LICENSE.txt
--rw-rw-r--   0 andy      (1000) andy      (1000)      460 2023-03-06 17:06:27.009531 cf-view-3.1.0/PKG-INFO
--rw-r--r--   0 andy      (1000) andy      (1000)      275 2021-05-19 13:18:16.000000 cf-view-3.1.0/README.txt
-drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-03-06 17:06:27.009531 cf-view-3.1.0/cf_view.egg-info/
--rw-rw-r--   0 andy      (1000) andy      (1000)      460 2023-03-06 17:06:26.000000 cf-view-3.1.0/cf_view.egg-info/PKG-INFO
--rw-rw-r--   0 andy      (1000) andy      (1000)      192 2023-03-06 17:06:26.000000 cf-view-3.1.0/cf_view.egg-info/SOURCES.txt
--rw-rw-r--   0 andy      (1000) andy      (1000)        1 2023-03-06 17:06:26.000000 cf-view-3.1.0/cf_view.egg-info/dependency_links.txt
--rw-rw-r--   0 andy      (1000) andy      (1000)       38 2023-03-06 17:06:26.000000 cf-view-3.1.0/cf_view.egg-info/requires.txt
--rw-rw-r--   0 andy      (1000) andy      (1000)        1 2023-03-06 17:06:26.000000 cf-view-3.1.0/cf_view.egg-info/top_level.txt
--rwxr-xr-x   0 andy      (1000) andy      (1000)   332967 2023-03-06 17:03:20.000000 cf-view-3.1.0/cfview
--rw-rw-r--   0 andy      (1000) andy      (1000)       38 2023-03-06 17:06:27.009531 cf-view-3.1.0/setup.cfg
--rw-r--r--   0 andy      (1000) andy      (1000)      804 2023-03-06 17:05:17.000000 cf-view-3.1.0/setup.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 10:12:50.705094 cf-view-3.2.22/
+-rw-r--r--   0 andy      (1000) andy      (1000)     1065 2021-06-09 09:47:44.000000 cf-view-3.2.22/LICENSE.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)      461 2023-05-18 10:12:50.705094 cf-view-3.2.22/PKG-INFO
+-rw-r--r--   0 andy      (1000) andy      (1000)      275 2021-05-19 13:18:16.000000 cf-view-3.2.22/README.txt
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-18 10:12:50.705094 cf-view-3.2.22/cf_view.egg-info/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      461 2023-05-18 10:12:50.000000 cf-view-3.2.22/cf_view.egg-info/PKG-INFO
+-rw-rw-r--   0 andy      (1000) andy      (1000)      192 2023-05-18 10:12:50.000000 cf-view-3.2.22/cf_view.egg-info/SOURCES.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)        1 2023-05-18 10:12:50.000000 cf-view-3.2.22/cf_view.egg-info/dependency_links.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)       38 2023-05-18 10:12:50.000000 cf-view-3.2.22/cf_view.egg-info/requires.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)        1 2023-05-18 10:12:50.000000 cf-view-3.2.22/cf_view.egg-info/top_level.txt
+-rwxr-xr-x   0 andy      (1000) andy      (1000)   366835 2023-05-18 10:10:47.000000 cf-view-3.2.22/cfview
+-rw-rw-r--   0 andy      (1000) andy      (1000)       38 2023-05-18 10:12:50.705094 cf-view-3.2.22/setup.cfg
+-rw-r--r--   0 andy      (1000) andy      (1000)      805 2023-05-18 10:11:04.000000 cf-view-3.2.22/setup.py
```

### Comparing `cf-view-3.1.0/LICENSE.txt` & `cf-view-3.2.22/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cf-view-3.1.0/cfview` & `cf-view-3.2.22/cfview`

 * *Files 4% similar despite different names*

```diff
@@ -22,22 +22,24 @@
 from PyQt5.QtCore import Qt, QObject, pyqtSignal, QAbstractTableModel, QVariant, QCoreApplication
 from PyQt5.QtGui import QFont, QPalette, QColor, QTextDocument, QPixmap, QImage, QStandardItemModel, QFontDatabase, QFontMetrics
 from copy import deepcopy
 from functools import partial
 from PIL import Image, ImageDraw
 from PIL.ImageQt import ImageQt
 import csv
+import json
 
 
 
 # Initiate the pvars class
 # This is used for storing plotting variables in plotvars
 class pvars(object):
+    '''The pvars object is used for storing plotting variables in plotvars'''
     def __init__(self, **kwargs):
-        '''Initialize a new Pvars instance'''
+        # Initialize a new Pvars instance
         for attr, value in kwargs.items():
             setattr(self, attr, value)
 
     def __str__(self):
         '''x.__str__() <==> str(x)'''
         a = None
         v = None
@@ -45,33 +47,32 @@
         for a, v in self.__dict__.items():
             return '\n'.join(out)
 
 cols = ['#abb6d4', '#7085c4', '#ffffff', '#f1f4fd', '#000000', '#000000']
 
 plotvars=pvars(pos=0, nplots=1, code='', plot_counter=0, title='', field_selected='',\
                file_selected=None, data=None, levs_automatic_set=True, levs_set=False,\
-               levs_manual_set=False, levs_min='0', levs_max='0', levs_step='0',levs_manual='',\
+               levs_manual_set=False, levs_min='', levs_max='', levs_step='',levs_manual='',\
                levs_extend_lower=True, levs_extend_upper=True, colorbar=True,\
                colorbar_orientation=None,\
                proj='cyl', lonmin='-180', lonmax='180', latmin='-90', latmax='90',\
                boundinglat='0', lon_0='0',
-               resolution='c', continent_thickness='1.5', continent_color='black',vect_title='',\
+               resolution='110m', continent_thickness='1.5', continent_color='black',vect_title='',\
                vect_ufield='', vect_auto_set=True, vect_key_length=10, vect_scale=100,\
                vect_stride='', vect_pts='', vect_stride_set=False,vect_pts_set=False,\
                vect_width = 0.02, vect_width_set=False, vect_headwidth = 3, vect_headwidth_set=False,\
-               cscales=None, cscale_automatic_set=True, cscale_reverse_set=False, cscale_white='',\
-               cscale_ncols='', cscale_above='', cscale_below='',cscale='viridis',\
+               cscales=None, cscale_automatic_set=True, cscale_reverse=False, cscale_white='',\
+               cscale_ncols='', cscale_above='', cscale_below='',cscale=None,\
                invalid_input=False, index_number=0, fields=None,\
                field__widget_indicies=None, field_widget_names=None, field_widget_title=None,\
                field_widget_listing='index', plot_type = 'Contour', contour_type='x-y', \
                collapse_x='Off', collapse_y='Off', collapse_z='Off', collapse_t='Off',\
                collapse_labels=['X', 'Y', 'Z', 'T'],\
                nx_length=None, ny_length=None, nz_length=None, nt_length=None,\
                stored = {},\
-               stored_dimensions=None, stored_collapses=None, stored_collapse_values=None,\
                stored_lock = False,\
                background_colour=cols[0], button_colour=cols[1], buttontext_colour=cols[2],\
                highlight_colour=cols[3], text_colour=cols[4], windowtext_colour=cols[5],\
                text_colour_insensitive = '#708090', font="DejaVu Sans", font_mono='DejaVu Sans Mono',\
                fontsize=15, fill=True, blockfill=False, lines=False, line_labels=False, titles=True,\
                blockfill_fast=False,\
                write_defaults=False, collapse_types=None, line_type='x', line_colour = 'C0',\
@@ -80,15 +81,15 @@
                line_markeredgecolor='', line_markeredgewidth='', line_limits='automatic',\
                trajectory_title='', trajectory_marker_shape='o', trajectory_marker_size='5',\
                trajectory_marker_face_colour='red', trajectory_marker_edge_colour='green', \
                trajectory_line_style='solid', trajectory_line_colour='blue', \
                trajectory_line_width='1.0', trajectory_vector=False, trajectory_legend=False,\
                trajectory_date_min='', trajectory_date_max='', dim_names=['x', 'y', 'z', 't'],\
                code_output=True, data_source_list=None, terminal_output=False, next_field_index=0,\
-               max_axes=10, nlevs=False)
+               max_axes=10, nlevs=False, maps_stored=None, levels_stored=None, scales_stored=None)
 
 
 cscales=['viridis', 'magma', 'inferno', 'plasma', 'parula', 'gray', 'hotcold_18lev', 'hotcolr_19lev',\
          'mch_default', 'perc2_9lev', 'percent_11lev', 'precip2_15lev', 'precip2_17lev', 'precip3_16lev',\
          'precip4_11lev', 'precip4_diff_19lev', 'precip_11lev', 'precip_diff_12lev', 'precip_diff_1lev', 'rh_19lev',\
          'spread_15lev', 'amwg', 'amwg_blueyellowred', 'BlueDarkRed18', 'BlueDarkOrange18', 'BlueGreen14', 'BrownBlue12',\
          'Cat12', 'cmp_flux', 'cosam12', 'cosam', 'GHRSST_anomaly', 'GreenMagenta16',\
@@ -117,37 +118,35 @@
 # Mac issue with pyqt5 as described at 
 # https://stackoverflow.com/questions/64833558/apps-not-popping-up-on-macos-big-sur-11-0-1
 # has resurfaced with pyqt5 = 4.19.18
 # pip install PyQt5==5.15.4 fixes it and also the following environment variable
 os.environ["QT_MAC_WANTS_LAYER"] = "1"
 
 class EmittingStream(QObject):
-
+    '''Class for output and errors'''
     textWritten = pyqtSignal(str)
 
     def write(self, text):
         self.textWritten.emit(str(text))
 
     def flush(self):
         pass
 
 
 def my_excepthook(type, value, tback):
-    # log the exception here
+    '''Log the exceptions'''
 
     # then call the default handler
     sys.__excepthook__(type, value, tback)
 
 sys.excepthook = my_excepthook
 
 
 class Cfview(QMainWindow):
-    '''
-     Main class for cfview
-    '''
+    '''Main window class for cfview'''
     def __init__(self, filename, defaults, parent=None):
         super(Cfview, self).__init__()
         plotvars.file_selected = filename
         
         # Set the file string in plotvars
         if plotvars.file_selected is not None:
             if len(plotvars.file_selected) == 1:
@@ -163,45 +162,87 @@
         self.parent = self
 
         # Read in the defaults file if it exists
         full_path = os.path.expanduser(defaults)
         check = os.path.isfile(full_path) 
 
         if check:
-            datafile = open(full_path, 'r')
-            for line in datafile:
-                vars = line.split(' ')
-                if line[0] != '#' and len(vars) > 1:
-                    var = vars[0]
-                    value = ''
-                    for i in np.arange(len(vars[1:])):
-                        if i > 0:
-                            value += ' ' 
-                        value += vars[i+1]
-                    value = value.replace("\n", "")
-
-                    if value == 'True':
-                        value = True
-                    if value == 'False':
-                        value = False
-            
-                    if var == 'fontsize':
-                        value = int(value)
+            with open(full_path, "r") as mydata:
+                my_defaults = json.load(mydata)
 
-                    setattr(plotvars, var, value)
+                for var in my_defaults:
+                    if var != 'maps' and var != 'levels':
+                        setattr(plotvars, var, my_defaults[var])
+                    else:
+                        for varmap in my_defaults['maps']['default']:
+                            setattr(plotvars, varmap, my_defaults['maps']['default'][varmap])
+                            
+                        if 'maps' in my_defaults:
+                            plotvars.maps_stored = my_defaults['maps']
+                            
+                        if 'levels' in my_defaults:
+                            plotvars.levels_stored = my_defaults['levels']
+                            
+                        if 'scales' in my_defaults:
+                            plotvars.scales_stored = my_defaults['scales']                   
+                            
+                            
         else:
             if defaults != '~/.cfview_defaults':
                 print("\nDefaults file " + defaults + " doesn't exist\n")
-
+                
+        # Set plotvars.maps_stored if it is not defined        
+        mymaps = plotvars.maps_stored
+        if mymaps is None:
+            mymaps = {}
+            mymaps['default'] = {}
+            mymaps['default']['lonmin'] = plotvars.lonmin
+            mymaps['default']['lonmax'] = plotvars.lonmax
+            mymaps['default']['latmin'] = plotvars.latmin
+            mymaps['default']['latmax'] = plotvars.latmax
+            mymaps['default']['proj'] = plotvars.proj
+            mymaps['default']['boundinglat'] = plotvars.boundinglat
+            mymaps['default']['lon_0'] = plotvars.lon_0
+            mymaps['default']['resolution'] = plotvars.resolution
+            mymaps['default']['continent_thickness'] = plotvars.continent_thickness
+            mymaps['default']['continent_color'] = plotvars.continent_color
+            plotvars.maps_stored = mymaps
+            
+        # Set plotvars.levels_stored if it is not defined        
+        mylevels = plotvars.levels_stored
+        if mylevels is None:
+            mylevels = {}
+            mylevels['default'] = {}
+            mylevels['default']['min'] = plotvars.levs_min
+            mylevels['default']['max'] = plotvars.levs_max
+            mylevels['default']['step'] = plotvars.levs_step
+            mylevels['default']['manual'] = plotvars.levs_manual
+            mylevels['default']['extend_lower'] = plotvars.levs_extend_lower
+            mylevels['default']['extend_upper'] = plotvars.levs_extend_upper
+            plotvars.levels_stored = mylevels
+            
+        # Set plotvars.scales_stored if it is not defined        
+        myscales = plotvars.scales_stored
+        if myscales is None:
+            myscales = {}
+            myscales['default'] = {}
+            myscales['default']['ncols'] = plotvars.cscale_ncols
+            myscales['default']['white'] = plotvars.cscale_white           
+            myscales['default']['above'] = plotvars.cscale_above
+            myscales['default']['below'] = plotvars.cscale_below
+            myscales['default']['reverse'] = plotvars.cscale_reverse
+            myscales['default']['cscale'] = plotvars.cscale       
+            plotvars.scales_stored = myscales
 
         self.initUI()
 
 
     def initUI(self):
-
+        ''' Main window layout '''
+        
         # Add a top menu bar
         bar = self.menuBar()
         # Turn off Mac bar relocation 
         bar.setNativeMenuBar(False)
 
         file = bar.addMenu("File")
         file.addAction("Open")
@@ -333,20 +374,14 @@
             self.lists_collapse[i].itemSelectionChanged.connect(self.reset_field_title)
             self.lists_collapse[i].setVisible(False)
 
         self.lists[0].setVisible(True)
             
 
 
-        # Set the stored_dimensions and stored_collapses for each of the fields in the field list
-        # -1 indicates that the dimension is unchanged by the user
-        plotvars.stored_dimensions = {}
-        plotvars.stored_collapses = {}
-        plotvars.stored_collapse_values = {}
-
 
 
         # Vector and contour and vector hbox
         contour_vector_indexHbox = QHBoxLayout()
         contour_indexLabel = QLabel('Contour Index')
         contour_indexComboBox = QComboBox()
         vector_x_indexLabel = QLabel('Vector x Index')
@@ -572,17 +607,15 @@
 
                 
         self.show()
         self.raise_()
 
 
     def open_file(self, s):
-        '''
-         Open a file and populate dimension lists
-        ''' 
+        '''Open a file dialog''' 
         dialog = QFileDialog()
         
         dialog.setOption(QFileDialog.DontUseNativeDialog, True)
         #dialog.setOption(QCoreApplication.AA_DontUseNativeDialogs, True)
         dialog.setAcceptMode(QFileDialog.AcceptOpen)
         #dialog.setNameFilters(["(*.nc *.pp)", "(*.nc)", "(*.pp)", "(*.*)"])
         dialog.setNameFilters(["*.nc *.pp", "*.nc", "*.pp", "*.*"])
@@ -614,17 +647,15 @@
         self.read_file(self)
         
 
 
 
 
     def read_file(self, s):
-        '''
-         Read file(s) and set widget values
-        '''
+        '''Read file(s), set widget values and populate plotvars.stored'''
     
         path = plotvars.file_selected
         
         try:
             if path != '':
                 f = cf.read(path)
             else:
@@ -634,14 +665,20 @@
             errstr = 'One of the files selected is not a valid, netCDF, PP or fields file or does not exist - '
             for file in path:
                 errstr += file + ' '
             print(errstr)
                 
             return
         
+        # Return if no fields are present
+        if len(f) == 0:
+            errstr = 'No fields are present in this file\n'
+            print(errstr)
+            return
+            
         
         plotvars.data_source_list = []
         for i in np.arange(len(f)):
             plotvars.data_source_list.append(plotvars.file_selected)
 
 
 
@@ -666,18 +703,16 @@
         plotvars.index_number = 0
         plotvars.fields = f
         plotvars.field_widget_indicies = None
         plotvars.next_field_index = len(f)
 
 
 
-        # Set the stored_dimensions
-        # -1 indicates that the dimension is unchanged
-        plotvars.stored_dimensions = {}
-        plotvars.stored_collapses = {}
+        # Set the stored values
+        # -1 indicates that the dimension or value is unchanged
         plotvars.stored = {}
         max_axes_number = 0
         maximum_axis_lengths = []
         
         if plotvars.file_selected is not None:
             for i in np.arange(len(f)):       
                                 
@@ -792,17 +827,15 @@
 
         # Print which file has been opened in the messages window
         print('File read: ' + str(path))
 
 
 
     def save_file(self, s):
-        '''
-         Save a file using selected fields, diemsion selections and collapses
-        '''
+        '''Save a file using selected fields, diemsion selections and collapses'''
 
         dialog = QFileDialog()
 
         dialog.setAcceptMode(QFileDialog.AcceptSave)
         dialog.setNameFilters(["netCDF Files (*.nc)", "All Files (*.*)"])
         dialog.setOption(QFileDialog.DontUseNativeDialog, True)
         #dialog.setOption(QCoreApplication.DontUseNativeDialogs, True)
@@ -840,17 +873,14 @@
         # Assemble the selected field indicies from the field titles
         selected = self.fieldlist.selectedItems()
         indicies = []
         for i in np.arange(len(selected)):
             field_title = selected[i].text()
             indicies.append(int(field_title.split()[0]))
 
-        #dims_regular = ['X', 'Y', 'Z', 'T']
-        #dims = Cf_funcs.find_dim_names(plotvars.fields[plotvars.index_number])
-
 
         save_fields = []
 
         # Set the data file
         f = plotvars.fields
 
         # Loop over the selected fields
@@ -919,15 +949,14 @@
                                 if ind < len(axis_indicies) - 1:
                                     com += ', ' 
                             com += '])\n'
 
 
             # Form the collapse string
             collapse_str = ''
-            #stored = plotvars.stored_collapses['f' + str(indicies[index])] 
             for i in np.arange(4):
                  if mycollapses[i] != 'Off':
                      collapse_str += data_axes[i] + ': ' + mycollapses[i] + ' '
             if len(collapse_str) > 0:
                 if collapse_str[-1] == ' ':
                     collapse_str = collapse_str[:-1]
 
@@ -956,17 +985,19 @@
            print('### Code to write the file is ###\n', com)
 
 
         
 
 
     def plot(self, s):
-        '''
-         Make a contour, vector, line or trajectory plot
-        '''
+        '''Make a contour, vector, line or trajectory plot'''
+        
+        
+        # Reset everything to clear any previous plot settings
+        cfp.reset()        
 
         index = plotvars.index_number
         if plotvars.plot_type == 'Contour and vector':
             index = self.contour_indexComboBox.currentIndex()
 
         # Return if no field
         if index == -1:
@@ -980,27 +1011,331 @@
         # Reset the file title in case the user has changed the field properties
         self.reset_field_title()
 
         # Check data and subspace if necessary
         subspace_args = {}
         con_args = {}
         
-        # ajh - to be removed
-        #dims = ['X', 'Y', 'Z', 'T']
-        
-        # ajh - new code 
         mystored = plotvars.stored['f' + str(index)]
               
         myaxes = deepcopy(mystored['data_axes'])
         
         for i in np.arange(len(myaxes)):
             if myaxes[i][:3] == 'dim':
                 myaxes[i] = 'dimensioncoordinate' + myaxes[i][3:]
         
+        
+
+        
+        # Assemble the map dictionary and associated cf-plot code if required
+        map_args = {}
+        setvars_args ={}
+        if (plotvars.plot_type in ['Contour', 'Vector', 'Contour and vector'] and  plotvars.contour_type == 'X-Y') or \
+            plotvars.plot_type == 'Trajectory' or plotvars.proj == 'rotated':
+
+            map_args = {}
+            setvars_args ={}
+            
+            if plotvars.proj == 'cyl':
+                # Check inputs are numbers
+                vals = [plotvars.lonmin, plotvars.lonmax, plotvars.latmin, plotvars.latmax]
+                vals_okay, errstr = Data_check.test_numbers(vals)
+                if not vals_okay:
+                    print('Error in cylindrical projection limits\n' + errstr)
+                    return
+
+                # Check lonmin < lonmax
+                vals = [plotvars.lonmin, plotvars.lonmax]
+                vals_okay, errstr = Data_check.test_ascending(vals)
+                if not vals_okay:
+                    myerr = 'Error in cylindrical projection longitude limits\n'
+                    myerr += 'lonmax must be > lonmin\n'
+                    print(myerr)
+                    return
+
+                # Check latmin < latmax
+                vals = [plotvars.latmin, plotvars.latmax]
+                vals_okay, errstr = Data_check.test_ascending(vals)
+                if not vals_okay:
+                    myerr = 'Error in cylindrical projection latitude limits\n'
+                    myerr += 'latmax must be > latmin\n'
+                    print(myerr)
+                    return
+
+
+                if float(plotvars.lonmin) != -180:
+                    map_args['lonmin'] = float(plotvars.lonmin)           
+                if float(plotvars.lonmax) != 180:
+                    map_args['lonmax'] = float(plotvars.lonmax)                              
+                if float(plotvars.latmin) != -90:
+                    map_args['latmin'] = float(plotvars.latmin)                           
+                if float(plotvars.latmax) != 90:
+                    map_args['latmax'] = float(plotvars.latmax)                              
+          
+                    
+
+            if plotvars.proj == 'spstere' or plotvars.proj == 'npstere':
+                # Check inputs are numbers
+                vals = [plotvars.boundinglat]
+                vals_okay, errstr = Data_check.test_numbers(vals)
+                if not vals_okay:
+                    print('Error in bounding latitude\n' + errstr)
+                    return
+
+                vals = [plotvars.lon_0]
+                vals_okay, errstr = Data_check.test_numbers(vals)
+                if not vals_okay:
+                    print('Error in longitude centre of map domain\n' + errstr)
+                    return
+
+                map_args['proj'] = plotvars.proj
+                if str(plotvars.boundinglat) != '0':
+                    map_args['boundinglat'] = float(plotvars.boundinglat)
+                if str(plotvars.lon_0) != '0':
+                    map_args['lon_0'] = float(plotvars.lon_0)
+
+
+
+            if plotvars.proj in ['EuroPP', 'lcc', 'merc', 'ortho', 'OSGB', 'robin', 'UKCP']:
+                map_args['proj'] = plotvars.proj
+                
+                if float(plotvars.lonmin) != -180.0 or float(plotvars.lonmax) != 180 or \
+                    float(plotvars.latmin) != -90.0 or float(plotvars.latmax) != 90:
+                    map_args['lonmin'] = float(plotvars.lonmin)
+                    map_args['lonmax'] = float(plotvars.lonmax)                   
+                    map_args['latmin'] = float(plotvars.latmin)                   
+                    map_args['latmax'] = float(plotvars.latmax) 
+
+
+            print('plotvars.proj is ', plotvars.proj)
+            
+            if plotvars.proj in ['rotated']:
+                if f.ref('grid_mapping_name:rotated_latitude_longitude', default=False):
+                    map_args['proj'] = 'rotated'
+
+            if plotvars.resolution != '110m':
+                map_args['resolution'] = plotvars.resolution
+                
+
+            # Setvars properties if changed
+            if plotvars.continent_thickness != '1.5':
+                setvars_args['continent_thickness'] = float(plotvars.continent_thickness)
+                
+            if plotvars.continent_color != 'black':
+                setvars_args['continent_color'] = plotvars.continent_color
+                
+        # Assemble the cf-plot code in map_com 
+        map_com = ''
+        vars = ['proj', 'lonmin', 'lonmax', 'latmin', 'latmax', 'boundinglat', 'lon_0', 'resolution']        
+        if len(map_args) > 0:
+            map_com = "cfp.mapset("
+            comma_count = 0
+            for i in np.arange(8):
+                if vars[i] in map_args:
+                    map_com += vars[i] + "="
+                if vars[i] in map_args and vars[i] in ['proj', 'resolution']:
+                    map_com += "'"
+                if vars[i] in map_args:    
+                    map_com += getattr(plotvars, vars[i])
+                    print('keyword and value are ', vars[i], getattr(plotvars, vars[i]))
+                if vars[i] in map_args and vars[i] in ['proj', 'resolution']:
+                    map_com += "'"                    
+                if vars[i] in map_args:                    
+                    comma_count += 1
+                    if comma_count < len(map_args) :
+                        map_com += ", "
+                        
+            map_com += ")"
+        
+        setvars_com = ''
+        if len(setvars_args) > 0:
+            setvars_com = "cfp.setvars("
+            if 'continent_thickness' in setvars_args:
+                setvars_com += 'continent_thickness=' + getattr(plotvars, 'continent_thickness')
+                if len(setvars_args) == 2:
+                    setvars_com += ', '
+            if 'continent_color' in setvars_args:
+                setvars_com += 'continent_color=' + getattr(plotvars, 'continent_color')
+    
+            setvars_com += ")"       
+        
+        
+        # Set up a levs_args dictionary and associated cf-plot code if required
+        cfp.levs()
+        levs_args = {}
+        levs_com = ''
+        
+        if plotvars.levs_extend_lower and plotvars.levs_extend_upper is False:
+            levs_args['extend'] = 'min'
+        if plotvars.levs_extend_lower is False and plotvars.levs_extend_upper:
+            levs_args['extend'] = 'max'                  
+        if plotvars.levs_extend_lower is False and plotvars.levs_extend_upper is False:
+            levs_args['extend'] = 'neither'  
+                     
+        if plotvars.levs_set:
+            vals = [plotvars.levs_min, plotvars.levs_max, plotvars.levs_step]
+
+            # Check all values are numbers
+            vals_okay, errstr = Data_check.test_numbers(vals)
+            if not vals_okay:
+                print('Error in evenly spaced contour levels\n' + errstr)
+                return
 
+            # Check min < max
+            vals_okay, errstr = Data_check.test_val0_lt_val1([vals[0], vals[1]])
+            if not vals_okay:
+                print('contour level error\n' + errstr)
+                return
+    
+            # Check step > 0
+            vals_okay, errstr = Data_check.test_val_gt_zero(vals[2])
+            if not vals_okay:
+                print('contour level step must be greater than zero\n')
+                return
+
+            # Test for ints or floats
+            all_ints, errstr = Data_check.test_integers(vals)
+                
+            if all_ints:
+                levs_args['min'] = int(vals[0])
+                levs_args['max'] = int(vals[1])
+                levs_args['step'] = int(vals[2])                    
+            else: 
+                levs_args['min'] = float(vals[0])
+                levs_args['max'] = float(vals[1])
+                levs_args['step'] = float(vals[2])                    
+                
+
+        elif plotvars.levs_manual_set:
+            # Check inputs are numbers
+            vals = plotvars.levs_manual.split(' ')
+            vals_okay, errstr = Data_check.test_numbers(vals)
+            if not vals_okay:
+                print('Error in manual contour levels\n' + errstr)
+                return
+
+
+            # Check inputs are ascending
+            vals_okay, errstr = Data_check.test_ascending(vals)
+            if not vals_okay:
+                print('Error in manual contour levels\n' + errstr)
+                return
+
+            # Check if all values are integers
+            myint, errstr = Data_check.test_integers(vals)
+
+
+            # Set up levels as a integer or float array
+            levels = []
+            for j in np.arange(np.size(vals)):
+                if myint:
+                    levels.append(int(vals[j]))
+                else:
+                    levels.append(float(vals[j]))
+
+            # Set up levels as a string array
+            levels_str = '['
+            for j in np.arange(np.size(vals)):
+                levels_str += vals[j]
+                if j < np.size(vals)-1:
+                    levels_str += ', '
+            levels_str += ']'
+
+            # Convert array to integer or float as appropriate
+            if myint:
+                levels = np.array(levels).astype(int)
+            else:
+                levels = np.array(levels).astype(float)
+
+            levs_args['manual'] = levels
+
+
+        if len(levs_args) > 0:
+            levs_com += 'cfp.levs('
+            if 'min' in levs_args and 'max' in levs_args and 'step' in levs_args:
+                levs_com += 'min=' + str(levs_args['min'])
+                levs_com += ', max=' + str(levs_args['max'])
+                levs_com += ', step=' + str(levs_args['step'])
+                
+            if 'manual' in levs_args:
+                levs_com += 'manual=['
+                for ilev in np.arange(len(levs_args['manual'])):
+                    levs_com += str(levs_args['manual'][ilev])
+                    if ilev < len(levs_args['manual']) - 1:
+                        levs_com += ', '
+                levs_com += ']'
+                
+            if 'extend' in levs_args:
+                levs_com += ", extend='" + levs_args['extend'] + "'" 
+            levs_com += ')\n'                
+
+        # Set up a colour cscale_args dictionary and associated cf-plot code if required
+        cfp.cscale()
+        cscale_args = {}
+        cscale_com = ''
+        
+        if plotvars.cscale_automatic_set is False:
+            
+            # Check any inputs are integers
+            if plotvars.cscale_ncols != '':
+                vals_okay, errstr = Data_check.test_integers(plotvars.cscale_ncols)
+                if not vals_okay:
+                    print('Error in colour scale numbers\n' + errstr)
+                    return
+
+            if plotvars.cscale_above != '':
+                vals_okay, errstr = Data_check.test_integers(plotvars.cscale_above)
+                if not vals_okay:
+                    print('Error in colour scale numbers\n' + errstr)
+                    return
+
+            if plotvars.cscale_below != '':
+                vals_okay, errstr = Data_check.test_integers(plotvars.cscale_below)
+                if not vals_okay:
+                    print('Error in colour scale numbers\n' + errstr)
+                    return
+
+            # Check white are numbers if specified
+            errstr = 'Error in colour white values\n'
+            white_vals = plotvars.cscale_white.split(' ')
+            if plotvars.cscale_white != '' and len(white_vals) > 0:
+                vals_okay, errstr = Data_check.test_integers(white_vals)
+                if not vals_okay:
+                    print('Error in colour scale white numbers\n' + errstr)
+                    return
+
+                white_vals = [int(i) for i in white_vals]
+                if len(white_vals) == 1:
+                    white_vals = white_vals[0]
+    
+    
+    
+        if plotvars.cscale != None:
+            cscale_args['scale'] = plotvars.cscale
+        if plotvars.cscale_ncols != '':
+            cscale_args['ncols'] = int(plotvars.cscale_ncols)
+        if plotvars.cscale_above != '':
+            cscale_args['above'] = int(plotvars.cscale_above)
+        if plotvars.cscale_below != '':
+            cscale_args['below'] = int(plotvars.cscale_below)
+        if plotvars.cscale_white != '':
+            cscale_args['white'] = white_vals
+        if plotvars.cscale_reverse:
+            cscale_args['reverse'] = True
+
+        if len(cscale_args) > 0:
+            cscale_com = 'cfp.cscale('
+            for key in cscale_args:
+                if key == 'scale':
+                    cscale_com += "scale='" + str(cscale_args[key]) + "',"
+                else: 
+                    cscale_com += str(key) + '=' + str(cscale_args[key]) + ','
+            cscale_com = cscale_com[:-1] + ')\n'
+        
+        
         if plotvars.plot_type == 'Contour' or plotvars.plot_type == 'Contour and vector':
             
             # Check selected data has enough items to be a contour plot
             axes = plotvars.contour_type.split('-')
             if len(axes) == 1 and axes[0] == '':
                 print('Not enough data to make a contour plot')
                 return
@@ -1047,19 +1382,19 @@
             # Form the subspace dictionary
             subspace_args = Cf_funcs.subspace_args(self.parent, index)
 
                  
             # Form the contour dictionary
             if plotvars.fill and not plotvars.lines:
                 con_args['lines'] = False
+                
             if not plotvars.fill and plotvars.lines:
                 con_args['fill'] = False
                 con_args['lines'] = True
 
-
             if plotvars.blockfill and not plotvars.lines:
                 con_args['blockfill'] = True
                 con_args['lines'] = False
 
             if plotvars.blockfill and plotvars.lines:
                 con_args['blockfill'] = True
                 con_args['lines'] = True
@@ -1114,267 +1449,43 @@
 
 
             # Set the map
             if plotvars.contour_type == 'X-Y':
                 cfp.mapset(proj=plotvars.proj)
 
 
-
             # Get the subspace and collapse commands
             com_subspace, com_collapse = Cf_funcs.com_subspace_collapse(subspace_args)
 
             # generate the code to read the data and apply subspace and collapse args
             variable_names = ['f', 'g', 'h']         
 
             com_con = Cf_funcs.generate_code(com_subspace, com_collapse)
 
             
 
             # Add contour levels if specified
-            if plotvars.levs_set:
-                vals = [plotvars.levs_min, plotvars.levs_max, plotvars.levs_step]
-
-                # Check all values are numbers
-                vals_okay, errstr = Data_check.test_numbers(vals)
-                if not vals_okay:
-                    print('Error in evenly spaced contour levels\n' + errstr)
-                    return
-
-                # Check min < max
-                vals_okay, errstr = Data_check.test_val0_lt_val1([vals[0], vals[1]])
-                if not vals_okay:
-                    print('contour level error\n' + errstr)
-                    return
-    
-                # Check step > 0
-                vals_okay, errstr = Data_check.test_val_gt_zero(vals[2])
-                if not vals_okay:
-                    print('contour level step must be greater than zero\n')
-                    return
-
-                # Test for ints or floats
-                all_ints, errstr = Data_check.test_integers(vals)
-                
-                # Set up levels and add to the com_con code
-                if all_ints:
-                    cfp.levs(min=int(vals[0]), max=int(vals[1]), step=int(vals[2]))
-                else:
-                    cfp.levs(min=float(vals[0]), max=float(vals[1]), step=float(vals[2]))
-                com_con += 'cfp.levs(min=' + vals[0] + ', max=' + vals[1] + ', step=' + vals[2] + ')\n'
-
-            elif plotvars.levs_manual_set:
-                # Check inputs are numbers
-                vals = plotvars.levs_manual.split(' ')
-                vals_okay, errstr = Data_check.test_numbers(vals)
-                if not vals_okay:
-                    print('Error in manual contour levels\n' + errstr)
-                    return
-
-
-                # Check inputs are ascending
-                vals_okay, errstr = Data_check.test_ascending(vals)
-                if not vals_okay:
-                    print('Error in manual contour levels\n' + errstr)
-                    return
-
-                # Check if all values are integers
-                myint, errstr = Data_check.test_integers(vals)
-
-
-                # Set up levels as a integer or float array
-                levels = []
-                for j in np.arange(np.size(vals)):
-                    if myint:
-                        levels.append(int(vals[j]))
-                    else:
-                        levels.append(float(vals[j]))
-
-                # Set up levels as a string array
-                levels_str = '['
-                for j in np.arange(np.size(vals)):
-                    levels_str += vals[j]
-                    if j < np.size(vals)-1:
-                        levels_str += ', '
-                levels_str += ']'
-
-                # Convert array to integer or float as appropriate
-                if myint:
-                    levels = np.array(levels).astype(int)
-                else:
-                    levels = np.array(levels).astype(float)
-
-
-                cfp.levs(manual=levels)
-                com_con += 'cfp.levs(manual=' + levels_str + ')\n'
-
-
-            elif plotvars.levs_automatic_set:
-                cfp.levs()
-
-
-
-            # Colour scale settings
-            if plotvars.cscale_automatic_set is False:
+            if len(levs_args) > 0:
+                cfp.levs(**levs_args)
+                com_con += levs_com
             
-                # Check any inputs are integers
-                if plotvars.cscale_ncols != '':
-                    vals_okay, errstr = Data_check.test_integers(plotvars.cscale_ncols)
-                    if not vals_okay:
-                        print('Error in colour scale numbers\n' + errstr)
-                        return
-
-                if plotvars.cscale_above != '':
-                    vals_okay, errstr = Data_check.test_integers(plotvars.cscale_above)
-                    if not vals_okay:
-                        print('Error in colour scale numbers\n' + errstr)
-                        return
-
-                if plotvars.cscale_below != '':
-                    vals_okay, errstr = Data_check.test_integers(plotvars.cscale_below)
-                    if not vals_okay:
-                        print('Error in colour scale numbers\n' + errstr)
-                        return
-
-
-                # Check white are numbers if specified
-                errstr = 'Error in colour white values\n'
-                white_vals = plotvars.cscale_white.split(' ')
-                if plotvars.cscale_white != '' and len(white_vals) > 0:
-                    vals_okay, errstr = Data_check.test_integers(white_vals)
-                    if not vals_okay:
-                        print('Error in colour scale white numbers\n' + errstr)
-                        return
-
-                    white_vals = [int(i) for i in white_vals]
-                    if len(white_vals) == 1:
-                        white_vals = white_vals[0]
-    
-
-
-
-            # Assemble the cscale command
-            # Reset cscale
-            cfp.cscale()
-
-            cscale_args = {}
-            if plotvars.cscale != 'viridis':
-                cscale_args['scale'] = plotvars.cscale
-            if plotvars.cscale_ncols != '':
-                cscale_args['ncols'] = int(plotvars.cscale_ncols)
-            if plotvars.cscale_above != '':
-                cscale_args['above'] = int(plotvars.cscale_above)
-            if plotvars.cscale_below != '':
-                cscale_args['below'] = int(plotvars.cscale_below)
-            if plotvars.cscale_white != '':
-                cscale_args['white'] = white_vals
-            if plotvars.cscale_reverse_set:
-                cscale_args['reverse'] = True
-
+            # Add colour scale if specified
             if len(cscale_args) > 0:
                 cfp.cscale(**cscale_args)
-                com_cscale = 'cfp.cscale('
-                for key in cscale_args:
-                    if key == 'scale':
-                        com_cscale += "cscale='" + str(cscale_args[key]) + "',"
-                    else: 
-                        com_cscale += str(key) + '=' + str(cscale_args[key]) + ','
-                com_cscale = com_cscale[:-1] + ')\n'
-                com_con += com_cscale
-            
-
-
-            # Map settings
-            # Reset map
-            cfp.mapset()
-
-            if plotvars.proj == 'cyl':
-                # Check inputs are numbers
-                vals = [plotvars.lonmin, plotvars.lonmax, plotvars.latmin, plotvars.latmax]
-                vals_okay, errstr = Data_check.test_numbers(vals)
-                if not vals_okay:
-                    print('Error in cylindrical projection limits\n' + errstr)
-                    return
-
-                # Check lonmin < lonmax
-                vals = [plotvars.lonmin, plotvars.lonmax]
-                vals_okay, errstr = Data_check.test_ascending(vals)
-                if not vals_okay:
-                    myerr = 'Error in cylindrical projection longitude limits\n'
-                    myerr += 'lonmax must be > lonmin\n'
-                    print(myerr)
-                    return
-
-                # Check latmin < latmax
-                vals = [plotvars.latmin, plotvars.latmax]
-                vals_okay, errstr = Data_check.test_ascending(vals)
-                if not vals_okay:
-                    myerr = 'Error in cylindrical projection latitude limits\n'
-                    myerr += 'latmax must be > latmin\n'
-                    print(myerr)
-                    return
-
-
-                if float(plotvars.lonmin) != -180.0 or float(plotvars.lonmax) != 180 or \
-                   float(plotvars.latmin) != -90.0 or float(plotvars.latmax) != 90:
-                    com_con += 'cfp.mapset(lonmin=' + str(plotvars.lonmin) + ', '
-                    com_con += 'lonmax=' + str(plotvars.lonmax) + ', '
-                    com_con += 'latmin=' + str(plotvars.latmin) + ', '
-                    com_con += 'latmax=' + str(plotvars.latmax) + ')\n'
-                    cfp.mapset(float(plotvars.lonmin), float(plotvars.lonmax), \
-                               float(plotvars.latmin), float(plotvars.latmax))
-
-
-
-            if plotvars.proj == 'spstere' or plotvars.proj == 'npstere':
-                # Check inputs are numbers
-                vals = [plotvars.boundinglat]
-                vals_okay, errstr = Data_check.test_numbers(vals)
-                if not vals_okay:
-                    print('Error in bounding latitude\n' + errstr)
-                    return
-
-                vals = [plotvars.lon_0]
-                vals_okay, errstr = Data_check.test_numbers(vals)
-                if not vals_okay:
-                    print('Error in longitude centre of map domain\n' + errstr)
-                    return
-
-                cfp.mapset(proj=plotvars.proj, boundinglat=float(plotvars.boundinglat),\
-                           lon_0 = float(plotvars.lon_0))
-
-                com_con += 'cfp.mapset(proj=' + plotvars.proj
-                if str(plotvars.boundinglat) != '0':
-                    com_con += ', boundinglat=' + str(plotvars.boundinglat)
-                if str(plotvars.lon_0) != '0':
-                    com_con += ', lon_0=' + plotvars.lon_0
-                com_con += ')\n'
-
-
-            if plotvars.proj in ['EuroPP', 'lcc', 'merc', 'ortho', 'OSGB', 'robin', 'UKCP', 'rotated']:
-                cfp.mapset(proj=plotvars.proj)
-                com_con += "cfp.mapset(proj='" + plotvars.proj + "')\n"
-
-
-            # Set continent properties if changed
-            if plotvars.continent_thickness != '1.5' or plotvars.continent_color != 'black':
-                cfp.setvars(continent_thickness=float(plotvars.continent_thickness),\
-                            continent_color=plotvars.continent_color)
-                continent_opts = 0
-                com_con += 'cfp.setvars('
-                if plotvars.continent_thickness != '1.5':
-                    com_con += 'continent_thickness=' + plotvars.continent_thickness
-                    continent_opts += 1
-                if plotvars.continent_color != 'black':
-                    if continent_opts != 0:
-                        com_con += ', '
-                    com_con += 'continent_color=' + plotvars.continent_color
-
-                com_con += ')\n'
- 
+                com_con += cscale_com
 
+            # Add map settings and code if specified
+            if len(map_args) > 0:
+                cfp.mapset(**map_args)
+                com_con += map_com + '\n'
+                
+            # Add setvars settings and code if specified
+            if len(setvars_args) > 0:
+                cfp.setvars(**setvars_args)
+                com_con += setvars_com + '\n'               
 
             com_con += 'cfp.con(' + 'f'
 
            
             if len(con_args) > 0:
                 for arg in con_args:
                     if arg != 'title':
@@ -1390,15 +1501,22 @@
                 if {'ax0', 'ax1', 'ax2', 'ax3'} > set(subspace_args):
                     axis_switch = True
                 
                 
             if axis_switch is False:
             
                 if len(subspace_args) > 0:
-                    f = f.subspace(**subspace_args)
+                    try:
+                        f = f.subspace(**subspace_args)
+                    except:
+                        errstr = 'Error in contour data subspace - check data is good'
+                        print(errstr)
+                        return
+
+
 
                 # Add bounds for those axes that need them
                 # ajh - new code
                 for i in np.arange(len(myaxes)):
                     if mystored['collapses'] != 'Off':
                         coord = f.coord(myaxes[i])
                         if len(coord.array) > 1:
@@ -1406,18 +1524,20 @@
                                 bounds = coord.create_bounds()
                                 coord.set_bounds(bounds)                
                 
                 
                 
                 
                 if com_collapse != '':
-                
-                    print('com_collapse is ', com_collapse)
-                    f = f.collapse(com_collapse.strip("'"), weights=True)
-
+                    try:
+                        f = f.collapse(com_collapse.strip("'"), weights=True)
+                    except:
+                        errstr = 'Error in contour data collapse - check data is good'
+                        print(errstr)
+                        return
 
                 # Use cfp.gopen if a contour and vector plot
                 if plotvars.plot_type == 'Contour and vector':
                     cfp.gopen()
                 
 
                 if plotvars.plot_type != 'Contour and vector':
@@ -1612,30 +1732,40 @@
                 com_line += 'ymin=' + plotvars.line_ymin + ', '
 
                 com_line += 'ymax=' + plotvars.line_ymax + ')\n'
 
               
             # Make the line plot            
             if len(subspace_args) > 0:
-                f = f.subspace(**subspace_args)
-
+                try:            
+                    f = f.subspace(**subspace_args)
+                except:
+                    errstr = 'Error in line data subspace - check data is good'
+                    print(errstr)
+                    return
                 
             # Add bounds for those axes that need them
             for i in np.arange(len(myaxes)):
                 if mystored['collapses'] != 'Off':
                     coord = f.coord(myaxes[i])
                     if len(coord.array) > 1:
                         if coord.has_bounds() is False:
                             bounds = coord.create_bounds()
                             coord.set_bounds(bounds)                          
                 
 
             
             if com_collapse != '':
-                f = f.collapse(com_collapse.strip("'"), weights=True)
+                try:
+                    f = f.collapse(com_collapse.strip("'"), weights=True)
+                except:
+                    errstr = 'Error in line data collapse - check data is good'
+                    print(errstr)
+                    return                    
+                    
 
             cfp.lineplot(f, **line_args)
 
             # Show the commands to make this line plot
             com_line += 'cfp.lineplot(' + 'f'
 
             if len(line_args) > 0:
@@ -1700,24 +1830,29 @@
 
             # Form the subspace dictionaries and apply if necessary
             u_subspace_args = Cf_funcs.subspace_args(self.parent, index_x)
             v_subspace_args = Cf_funcs.subspace_args(self.parent, index_y)
 
             u = deepcopy(plotvars.fields[index_x])
             if len(u_subspace_args) > 0:
-                u = u.subspace(**u_subspace_args)
-
+                try:
+                    u = u.subspace(**u_subspace_args)
+                except:
+                    errstr = 'Error in vector u data subspace - check data is good'
+                    print(errstr)
+                    return
+                    
             v = deepcopy(plotvars.fields[index_y])
             if len(v_subspace_args) > 0:
-                v = v.subspace(**v_subspace_args)
-
-            # Set the map
-            if plotvars.contour_type == 'x-y':
-                cfp.mapset(proj=plotvars.proj)
-
+                try:
+                    v = v.subspace(**v_subspace_args)
+                except:
+                    errstr = 'Error in vector v data subspace - check data is good'
+                    print(errstr)
+                    return
 
 
             # Assemble vector arguments
             vect_args = {}
                             
             if plotvars.vect_title == '':
                 vect_args['titles'] = True
@@ -1789,14 +1924,29 @@
             else:
                 com_u = Cf_funcs.generate_code(ucom_subspace, ucom_collapse, index=index_x, var_index=1)
                 com_v = Cf_funcs.generate_code(vcom_subspace, vcom_collapse, index=index_y, var_index=2)
                 
             
             com += com_u + com_v
 
+
+
+            # Map settings and code if required
+            cfp.mapset()
+            if len(map_args) > 0:
+                cfp.mapset(**map_args)
+                com += map_com + '\n'
+                
+            # setvars settings and code if required
+            if len(setvars_args) > 0:
+                cfp.setvars(**setvars_args)
+                com += setvars_com + '\n' 
+
+
+
             # Assemble the cfp.vect command
             if plotvars.plot_type == 'Vector':
                 vect_com = 'cfp.vect(u=f, v=g'
             else:
                 vect_com = 'cfp.vect(u=g, v=h'
 
             for arg in vect_args:
@@ -1820,14 +1970,15 @@
 
             cfp.vect(u=u, v=v, **vect_args)
 
 
             if plotvars.plot_type == 'Contour and vector':
                 cfp.gclose()
 
+
         if plotvars.plot_type == 'Trajectory':
 
             traj_args = {}
             com_traj = 'import cf\n'
             com_traj += 'import cfplot as cfp\n'
 
             index = plotvars.index_number
@@ -1869,76 +2020,23 @@
 
 
 
             # Map settings
             # Reset map
             cfp.mapset()
 
-            if plotvars.proj == 'cyl':
-                # Check inputs are numbers
-                vals = [plotvars.lonmin, plotvars.lonmax, plotvars.latmin, plotvars.latmax]
-                vals_okay, errstr = Data_check.test_numbers(vals)
-                if not vals_okay:
-                    print('Error in cylindrical projection limits\n' + errstr)
-                    return
-
-                # Check lonmin < lonmax
-                vals = [plotvars.lonmin, plotvars.lonmax]
-                vals_okay, errstr = Data_check.test_ascending(vals)
-                if not vals_okay:
-                    myerr = 'Error in cylindrical projection longitude limits\n'
-                    myerr += 'lonmax must be > lonmin\n'
-                    print(myerr)
-                    return
-
-                # Check latmin < latmax
-                vals = [plotvars.latmin, plotvars.latmax]
-                vals_okay, errstr = Data_check.test_ascending(vals)
-                if not vals_okay:
-                    myerr = 'Error in cylindrical projection latitude limits\n'
-                    myerr += 'latmax must be > latmin\n'
-                    print(myerr)
-                    return
-
-
-                if float(plotvars.lonmin) != -180.0 or float(plotvars.lonmax) != 180 or \
-                   float(plotvars.latmin) != -90.0 or float(plotvars.latmax) != 90:
-                    com_traj += 'cfp.mapset(lonmin=' + str(plotvars.lonmin) + ', '
-                    com_traj += 'lonmax=' + str(plotvars.lonmax) + ', '
-                    com_traj += 'latmin=' + str(plotvars.latmin) + ', '
-                    com_traj += 'latmax=' + str(plotvars.latmax) + ')\n'
-                    cfp.mapset(float(plotvars.lonmin), float(plotvars.lonmax), \
-                               float(plotvars.latmin), float(plotvars.latmax))
-
-
-
-            if plotvars.proj == 'npstere' or plotvars.proj == 'spstere':
-                # Check inputs are numbers
-                vals = [plotvars.boundinglat]
-                vals_okay, errstr = Data_check.test_numbers(vals)
-                if not vals_okay:
-                    print('Error in bounding latitude\n' + errstr)
-                    return
-
-                vals = [plotvars.lon_0]
-                vals_okay, errstr = Data_check.test_numbers(vals)
-                if not vals_okay:
-                    print('Error in longitude centre of map domain\n' + errstr)
-                    return
-
-
-                cfp.mapset(proj=plotvars.proj, boundinglat=float(plotvars.boundinglat),\
-                           lon_0 = float(plotvars.lon_0))
-
-                com_traj += 'cfp.mapset(proj=' + plotvars.proj
-                if str(plotvars.boundinglat) != '0':
-                    com_traj += ', boundinglat=' + str(plotvars.boundinglat)
-                if str(plotvars.lon_0) != '0':
-                    com_traj += ', lon_0=' + plotvars.lon_0
-                com_traj += ')\n'
+            # Map settings and code if required 
+            if len(map_args) > 0:
+                cfp.mapset(**map_args)
+                com_traj += map_com + '\n'
+                
+            # setvars settings and code if required
+            if len(setvars_args) > 0:
+                cfp.setvars(**setvars_args)
+                com_traj += setvars_com + '\n'  
                 
 
 
             if plotvars.trajectory_legend:
                 if plotvars.levs_set:
 
                     vals = [plotvars.levs_min, plotvars.levs_max, plotvars.levs_step]
@@ -2046,17 +2144,15 @@
             if plotvars.code_output:
                 print('*** Code to make plot is ***\n', com_traj)
 
 
 
 
     def fieldnumber(self):
-        '''
-         Change the field number 
-        '''
+        '''Change the field number '''
 
         # Find out which fields are selected.
         # If multiple fields then select the first.
         selected = self.fieldlist.selectedItems()
         if len(selected) == 0:
             return
 
@@ -2169,15 +2265,30 @@
         for axis in myaxes:
             l_options.append(axis)
         self.line_type_ComboBox.addItems(l_options)
         self.line_type_ComboBox.setCurrentIndex(line_index)
         plotvars.line_type = str(self.line_type_ComboBox.currentText())
 
 
-        # If the data_window is open reset the data type dropdown 
+        # If map_window is open reset the data type dropdown 
+        if self.map_window:
+        
+            obj = self.map_window.rotatedCheckBox
+            pal = QPalette(obj.palette())
+            
+            if plotvars.fields[plotvars.index_number].ref('grid_mapping_name:rotated_latitude_longitude', default=False):
+                obj.setEnabled(True)
+                pal.setColor(QPalette.WindowText, QColor(plotvars.text_colour))
+            else:
+                obj.setEnabled(False)
+                pal.setColor(QPalette.WindowText, QColor(plotvars.text_colour_insensitive))    
+                            
+            obj.setPalette(pal)         
+
+        # If data_window is open reset the data type dropdown 
         if self.data_window:
 
             # Reset the data
             Populate_table(self.data_window, initial = False)
             
             self.data_window.data_ComboBox.clear()
             
@@ -2218,29 +2329,24 @@
         self.lists[0].setVisible(True)
                     
         # Add the reset dimension button
         getattr(self, 'rightHbox3').addWidget(getattr(self, 'reset_dimensionButton'))
 
 
     def dim_traj_reset(self, option):
-        '''
-         Reset the dimension or trajectory selection to all
-        '''
+        '''Reset the dimension or trajectory selection'''
         
         if plotvars.fields is None:
             return
         if len(plotvars.fields) == 0:
             return
             
         f = deepcopy(plotvars.fields[plotvars.index_number])
         
-        
-        # ajh - new code
         index_str = 'f' + str(plotvars.index_number)
-        
         axis_vals = Cf_funcs.field_axis_values(field=f)
         
         
         mystored = plotvars.stored[index_str]
         myaxes = mystored['data_axes']
         
         
@@ -2308,35 +2414,29 @@
         
         # Reset the field title
         self.reset_field_title()       
 
 
 
     def contour_type(self, text):
-        '''
-         Set the contour plot type in plotvars
-        '''
+        '''Set the contour plot type in plotvars'''
 
         plotvars.contour_type = text
         
 
 
     def line_type(self, text):
-        '''
-         Set the line plot type in plotvars
-        '''
+        '''Set the line plot type in plotvars'''
 
         plotvars.line_type = text
 
 
 
     def plot_type(self, text):
-        '''
-         Set the contour plot type in plotvars
-        '''
+        '''Set the contour plot type in plotvars'''
         plotvars.plot_type = text
 
         objs = [self.contour_indexLabel, self.contour_indexComboBox,
         self.vector_x_indexLabel, self.vector_x_indexComboBox,
         self.vector_y_indexLabel, self.vector_y_indexComboBox]
 
         # Clear contour and vector comboboxes and repopulate
@@ -2381,18 +2481,15 @@
                 obj.setVisible(False)
 
 
  
 
 
     def dim_view(self, iaxis):
-
-        '''    
-         Set the visible state of the dimension lists and lists_collapse 
-        '''
+        '''Set the visible state of the dimension lists and lists_collapse '''
                       
         # Turn RadioButton and list visibilty off
         for i in np.arange(plotvars.max_axes):
             self.axis_RadioButtons[i].setChecked(False)
             self.lists[i].setVisible(False)
             self.lists_collapse[i].setVisible(False)
             
@@ -2403,17 +2500,15 @@
             self.lists[iaxis].setVisible(True)
         else:
             self.lists_collapse[iaxis].setVisible(True)
 
 
 
     def field_widget_listing(self, listing):
-        '''
-         Change field widget listing based on order or name
-        '''
+        '''Change field widget listing based on order or name'''
 
 
 
         plotvars.field_widget_listing = listing
 
         listings = ['index', 'field']
         ticked_state = [False, False]
@@ -2430,46 +2525,41 @@
         for i in np.arange(len(field_widget_names)):
             QListWidgetItem(field_widget_names[i], self.fieldlist) 
         self.fieldlist.setCurrentRow(0)
         self.field_titles.setText(field_widget_title)
 
 
     def search_fields(self, text):
-        '''
-         change field list based on search
+        '''Change field list based on search
         '''
         field_widget_names, field_widget_title = Cf_funcs.fields_list(self, order=plotvars.field_widget_listing,
                                                  order_changed=True, search=text)
 
         self.fieldlist.clear()
         for i in np.arange(len(field_widget_names)):
             QListWidgetItem(field_widget_names[i], self.fieldlist) 
         self.fieldlist.setCurrentRow(0)
         self.field_titles.setText(field_widget_title)
 
 
 
     def output_terminal_written(self, text):
-        '''
-         Output any text to the cfview output text panel
-        '''
+        '''Output any text to the cfview output text panel'''
 
         self.output_terminal_textEdit.append(text)
 
 
     
     
              
 
 
 
     def reset_field_title(self):
-        '''
-         Reset the field title
-        '''
+        '''Reset the field title'''
 
         # Return if no fieldlist or if plotvars.fields is None
         if not hasattr(self, 'fieldlist') or plotvars.fields is None:
             return
 
 
         # Check if this field is a trajectory
@@ -2757,15 +2847,15 @@
         if value.text() == 'transform':
             if self.transform_window is None:
                 self.transform_window = Transform_window(self.parent)
             self.transform_window.show()
 
         if value.text() == 'about':
             html = '<body><h2>About cfview</h2>'
-            html += '<b>This is version 3.0.0</b><p>'
+            html += '<b>This is version 3.2.22</b><p>'
             html += 'cfview is a quick look data exploration tool for netCDF, Met Office PP and fields file data'
             html += '<p>'
             html += 'cfview uses:<br>'
             html += '<b>cf-python</b> - data I/O and manipulation<br>'
             html += 'https://ncas-cms.github.io/cf-python<p>'
             html += '<b>cf-plot</b> - plotting<br>'
             html += 'http://ajheaps.github.io/cf-plot<P>'
@@ -2813,43 +2903,45 @@
 
 
 
             self.cfview_help = Help(html)
             self.cfview_help.show()
 
     def file_menu(self, value):
-
+        '''Open requested menu item'''
+        
         if value.text() == 'Open':
             self.open_file(self)
 
         if value.text() == 'Save':
             self.save_file(self)
 
         if value.text() == 'Exit':
             sys.exit(0)
 
 
 
 
 class Cfview_defaults_window(QWidget):
-    '''popup window for editing cfview defaults'''
+    '''Popup window for editing cfview defaults'''
 
     def __init__(self, parent):
         super(Cfview_defaults_window, self).__init__()
 
         self.parent = parent
         self.initUI()
         
         self.windows = ['trajectory_window', 'names_window', 'transform_window', 'vector_window',\
                         'data_window', 'line_window', 'contour_window', 'map_window', \
                         'colour_scale', 'contour_levels']
 
 
     def initUI(self):
-
+        ''' Main window layout '''
+        
         # Set up some buttons
         resetButton = QPushButton("Reset")
         resetButton.clicked.connect(self.reset)
         helpButton = QPushButton("Help")
         helpButton.clicked.connect(self.help)
         saveButton = QPushButton("Save defaults to file:")
         saveButton.clicked.connect(self.save)
@@ -3004,15 +3096,16 @@
         self.window().setFont(custom_font)
 
         self.defaults_help = None  # No external window yet.
 
         self.show()
 
     def theme(self, name):
-
+        '''Define the colour themes'''
+        
         cols = ['#f5deb3', '#f5deb3', '#000000', '#bfdfff', '#000000', '#000000']
 
         if name == 'BlueMono':
             cols = ['#abb6d4', '#7085c4', '#ffffff', '#f1f4fd', '#000000', '#000000']
 
         if name == 'BluePurple':
             cols = ['#a5cadd', '#313852', '#ffffff', '#dff5ff', '#000000', '#7a2894']
@@ -3082,15 +3175,15 @@
         for window in self.windows: 
             if getattr(self.parent, window):
                 getattr(self.parent, window).setPalette(palette)
             
 
 
     def fontsize(self):
-
+        '''Set the font size'''
         value = self.font_Slider.value()
         font = QFont(plotvars.font, value)
 
         self.parent.window().setFont(font)
         plotvars.fontsize = value
         self.font_size_Label.setText('Font size: ' + str(value))
 
@@ -3098,50 +3191,52 @@
         self.parent.window().fieldlist.setFont(font)
         
         self.parent.window().field_titles.setFont(font)
         self.parent.window().fieldlist.setFont(font)
         
 
     def font_main(self, value):
-
+        '''Set the main font'''
         plotvars.font = value
         font = QFont(plotvars.font, plotvars.fontsize)
         self.parent.window().setFont(font)
         
 
     def font_mono(self, value):
-
+        '''Set the mono font'''
         plotvars.font_mono = value
         font = QFont(plotvars.font_mono, plotvars.fontsize)
 
         # Set mono font for field titles and field list
         self.parent.window().field_titles.setFont(font)
         self.parent.window().fieldlist.setFont(font)
 
 
     def code_output(self):
+        '''Set the code output in plotvars'''
         if self.code_outputCheckBox.isChecked():
             plotvars.code_output = True
         else:
             plotvars.code_output = False
             
             
     def terminal_output(self):
+        '''Set the terminal output'''
         if self.terminal_outputCheckBox.isChecked():
             plotvars.terminal_output = True
             sys.stdout = sys.__stdout__
             sys.stderr = sys.__stderr__
         else:
             plotvars.terminal_output = False        
             sys.stdout = EmittingStream(textWritten=self.parent.output_terminal_written)
             sys.stderr = EmittingStream(textWritten=self.parent.output_terminal_written)
             
 
     def reset(self):
-        # Reset to defaults
+        '''Reset to defaults'''
         self.saveTextBox.setText('~/.cfview_defaults')
         plotvars.fontsize = 15
         self.font_Slider.setValue(15)
         self.font_size_Label.setText('Font size: 15')
 
         # Find available fonts
         db = QFontDatabase()
@@ -3179,16 +3274,15 @@
         
          # Terminal output is True
         self.terminal_outputCheckBox.setChecked(False)
         plotvars.terminal_output = True       
         
 
     def save(self):
-
-        # Ask to clobber existing file
+        '''Ask whether to clobber existing file'''
         full_path = os.path.expanduser(self.saveTextBox.text())
         self.savefile = full_path
         check = os.path.isfile(full_path) 
         
         if check:
             html = ''
             html += '<body>The file ' + full_path + ' already exists'
@@ -3202,15 +3296,15 @@
         else:
             plotvars.write_defaults = True
             
         Save_defaults(self.savefile)
 
 
     def help(self):
-
+        '''Help fr cfview defaults'''
         if self.defaults_help is None:
 
             html = ''
             html += '<body><h2>cfview default options</h2>'
             html += 'The defaults file for cfview is generally stored in the file ~/.cfview_defaults '
             html += 'which is read in when cfview starts up.  A different defaults file can be specified using '
             html += 'the -d parameter to the cfview command line i.e.<br>'
@@ -3224,15 +3318,15 @@
 
             self.defaults_help = Help(html)
 
         self.defaults_help.show()
         
         
     def closeEvent(self, event):
-        # Close self.parent.cfview_defaults_window
+        '''Close self.parent.cfview_defaults_window'''
         self.parent.cfview_defaults_window = None
         self.close()
         
 
 
 class Clobber_file(QWidget):
     '''Popup window for clobbering a file'''
@@ -3241,15 +3335,16 @@
         super(Clobber_file, self).__init__()
         self.html = html
         self.savefile = savefile
         self.initUI()
 
 
     def initUI(self):
-
+        ''' Main window layout '''
+        
         yesButton = QPushButton("Yes")
         yesButton.clicked.connect(self.clobber_yes)
 
         noButton = QPushButton("No")
         noButton.clicked.connect(self.clobber_no)
 
         helpTextbox = QTextEdit()
@@ -3290,82 +3385,106 @@
 
         self.setFixedWidth(600)
 
         self.show()
 
 
     def clobber_yes(self):
+        '''Clobber and save file'''
         plotvars.write_defaults = True
-        #self.savefile()
         Save_defaults(self.savefile)
         self.close()
 
     def clobber_no(self):
+        '''Don't clobber and exit'''
         plotvars.write_defaults = False
         self.close()
 
      
 
 class Save_defaults():
-
+    '''Save defults class'''
+    
     def __init__(self, savefile):
         super(Save_defaults, self).__init__()
         self.savefile = savefile
         self.save()
 
     def save(self):
+        '''Save the defaults'''
         if plotvars.write_defaults:
-        
+            
             plotvars.write_defaults = False
+            
+            my_defaults = {}
+            my_defaults['background_colour'] = plotvars.background_colour
+            my_defaults['button_colour'] = plotvars.button_colour
+            my_defaults['buttontext_colour'] = plotvars.buttontext_colour
+            my_defaults['highlight_colour'] = plotvars.highlight_colour
+            my_defaults['text_colour'] = plotvars.text_colour
+            my_defaults['font'] = plotvars.font
+            my_defaults['font_mono'] = plotvars.font_mono
+            my_defaults['fontsize'] = plotvars.fontsize        
+            my_defaults['fill'] = plotvars.fill 
+            my_defaults['code_output'] = plotvars.code_output        
+            my_defaults['terminal_output'] = plotvars.terminal_output
+            my_defaults['blockfill'] = plotvars.blockfill      
+            my_defaults['blockfill_fast'] = plotvars.blockfill_fast    
+            my_defaults['lines'] = plotvars.lines       
+            my_defaults['line_labels'] = plotvars.line_labels
+            my_defaults['titles'] = plotvars.titles
+            my_defaults['nlevs'] = plotvars.nlevs         
+            
+            my_defaults['maps'] = plotvars.maps_stored
+            my_defaults['levels'] = plotvars.levels_stored           
+            my_defaults['scales'] = plotvars.scales_stored                       
 
-            datafile = open(self.savefile, 'w')
-            datafile.write('### cfview defaults file ###\n\n')
-            datafile.write('background_colour ' + plotvars.background_colour + '\n')
-            datafile.write('button_colour ' + plotvars.button_colour + '\n')
-            datafile.write('buttontext_colour ' + plotvars.buttontext_colour + '\n')
-            datafile.write('highlight_colour ' + plotvars.highlight_colour + '\n')
-            datafile.write('text_colour ' + plotvars.text_colour + '\n')
-            datafile.write('windowtext_colour ' + plotvars.windowtext_colour + '\n')
-            datafile.write('font ' + plotvars.font + '\n')
-            datafile.write('font_mono ' + plotvars.font_mono + '\n')
-            datafile.write('fontsize ' + str(plotvars.fontsize) + '\n')
-            datafile.write('fill ' + str(plotvars.fill) + '\n')
-            datafile.write('code_output ' + str(plotvars.code_output) + '\n')
-            datafile.write('terminal_output ' + str(plotvars.terminal_output) + '\n')
-            datafile.write('blockfill ' + str(plotvars.blockfill) + '\n')
-            datafile.write('blockfill_fast ' + str(plotvars.blockfill_fast) + '\n')
-            datafile.write('lines ' + str(plotvars.lines) + '\n')
-            datafile.write('line_labels ' + str(plotvars.line_labels) + '\n')
-            datafile.write('titles ' + str(plotvars.titles) + '\n')
-            datafile.write('nlevs ' + str(plotvars.nlevs) + '\n')            
-            datafile.close()
-
+            with open(self.savefile, "w") as mysave:
+                json.dump(my_defaults, mysave)
 
 
+            
 class Contour_levels_window(QWidget):
-    '''popup window for editing contour level defaults'''
+    '''Popup window for editing contour level defaults'''
 
     def __init__(self, parent):
         super(Contour_levels_window, self).__init__()
 
         self.parent = parent
         self.initUI()
 
 
     def initUI(self):
-
+        ''' Main window layout '''
+        
         # Set up some buttons
         resetButton = QPushButton("Reset")
         resetButton.clicked.connect(self.reset)
 
         helpButton = QPushButton("Help")
         helpButton.clicked.connect(self.help)
 
         quitButton = QPushButton("Quit")
         quitButton.clicked.connect(self.closeEvent)
+        
+        save_levelsButton = QPushButton('Save settings to this levels name:')
+        save_levelsButton.clicked.connect(self.save_levels)
+        save_settingsButton = QPushButton('Save all cfview settings to this file:')
+        save_settingsButton.clicked.connect(self.save_settings)
+        delete_levelsButton = QPushButton('Delete currently selected levels')
+        delete_levelsButton.clicked.connect(self.delete_levels)
+        
+        # Set up user levels dropdown
+        user_levelsComboBox = QComboBox()
+        mylevels = plotvars.levels_stored
+        for mylevel in mylevels:
+            user_levelsComboBox.addItem(mylevel)
+        user_levelsComboBox.activated[str].connect(self.user_levels_changed)
+        self.user_levelsComboBox = user_levelsComboBox
+
 
         # Labels
         automatic_Label = QLabel('Automatic levels')
 
         min_Label = QLabel('Min:')
         min_Label.setEnabled(False)
         max_Label = QLabel('Max:')
@@ -3373,14 +3492,15 @@
         step_Label = QLabel('Step:')
         step_Label.setEnabled(False)
 
         ascending_Label = QLabel('Ascending values separated by spaces')
         extensions_Label = QLabel('Colourbar extensions - extend contours to cover all the data')
         lower_Label = QLabel('Lower:')
         upper_Label = QLabel('Upper:')
+        user_levelsLabel = QLabel('User levels:')
 
 
         # Level type selection tick boxes
         automaticCheckBox = QCheckBox("Automatic levels")
         automaticCheckBox.setChecked(True)
         automaticCheckBox.clicked.connect(lambda: self.level_type('automatic'))
 
@@ -3416,15 +3536,32 @@
         levs_stepTextbox.setEnabled(True)
 
         levs_manualTextbox = QLineEdit()
         levs_manualTextbox.textChanged.connect(self.levs_manual_changed)
         levs_manualTextbox.setEnabled(True)
 
 
+        save_levelsTextBox = QLineEdit()
+        save_settingsTextBox = QLineEdit()
+        save_settingsTextBox.setText('~/.cfview_defaults')
+
+        self.save_levelsTextBox = save_levelsTextBox
+        self.save_settingsTextBox = save_settingsTextBox
+
+
+
+
         vbox = QVBoxLayout()
+        
+        # User defined levels
+        hbox_levels = QHBoxLayout()
+        hbox_levels.addWidget(user_levelsLabel)
+        hbox_levels.addWidget(user_levelsComboBox)
+        vbox.addLayout(hbox_levels)
+
         hbox_even = QHBoxLayout()
         hbox_manual = QHBoxLayout()
         hbox_extensions = QHBoxLayout()
         hbox_buttons = QHBoxLayout()
 
         vbox.addWidget(automaticCheckBox)
         vbox.addWidget(HLine())
@@ -3445,35 +3582,93 @@
         hbox_manual.addWidget(levs_manualTextbox)
 
         vbox.addWidget(HLine())
         vbox.addWidget(extensions_Label)
         vbox.addLayout(hbox_extensions)
         hbox_extensions.addWidget(extension_lowerCheckBox)
         hbox_extensions.addWidget(extension_upperCheckBox)
+        
+        vbox.addWidget(HLine())    
+        
+        # Saving levels options
+        user_managementCheckBox = QCheckBox('View user level management options')
+        user_managementCheckBox.clicked.connect(partial(self.level_management, 'clicked'))
+        self.user_managementCheckBox = user_managementCheckBox
+        
 
-        vbox.addLayout(hbox_buttons)
+        # User levels management
+        vbox.addWidget(user_managementCheckBox)
+        
+        # Put management options in a frame as this can be hidden whereas a QVBoxLayout cannot 
+        management_frame = QFrame()
+        
+        vbox2 = QVBoxLayout()        
+        
+
+        hbox_save_levels = QHBoxLayout()
+        hbox_save_levels.addWidget(save_levelsButton)
+        hbox_save_levels.addWidget(save_levelsTextBox)
+        vbox2.addLayout(hbox_save_levels)
+
+        hbox_save_settings = QHBoxLayout()
+        hbox_save_settings.addWidget(save_settingsButton)
+        hbox_save_settings.addWidget(save_settingsTextBox)
+        vbox2.addLayout(hbox_save_settings)
+
+        hbox_delete_levels = QHBoxLayout()
+        hbox_delete_levels.addWidget(delete_levelsButton)
+        hbox_delete_levels.addStretch(1)
+        vbox2.addLayout(hbox_delete_levels)
+
+        management_frame.setLayout(vbox2)
+        management_frame.hide()
+        self.management_frame = management_frame
+        vbox.addWidget(management_frame)        
+        
+        
+        
+        
         hbox_buttons.addWidget(resetButton)
         hbox_buttons.addWidget(helpButton)
         hbox_buttons.addWidget(quitButton)
 
    
         self.setWindowTitle('cfview contour levels')
 
-        self.setLayout(vbox)
+
+        # Make a scrollable area
+        groupBox = QGroupBox('')
+        groupBox.setLayout(vbox)
+        scroll = QScrollArea()
+        scroll.setWidget(groupBox)
+        scroll.setWidgetResizable(True)
+        vscroll = scroll.verticalScrollBar()
+        #scroll.setFixedWidth(800)
+        #scroll.setFixedHeight(800)
+        container = QVBoxLayout()
+        container.addWidget(scroll)
+
+        container.addLayout(hbox_buttons)
+        
+        self.scroll = scroll
+        self.vscroll = vscroll
+        self.setLayout(container)
+
+
 
 
         self.automaticCheckBox = automaticCheckBox
         self.evenCheckBox = evenCheckBox
         self.levs_minTextbox = levs_minTextbox
         self.levs_maxTextbox = levs_maxTextbox
         self.levs_stepTextbox = levs_stepTextbox
         self.manualCheckBox = manualCheckBox
         self.levs_manualTextbox = levs_manualTextbox
-        self.extension_lowerCheck = extension_lowerCheckBox
-        self.extension_upperCheck = extension_upperCheckBox
+        self.extension_lowerCheckBox = extension_lowerCheckBox
+        self.extension_upperCheckBox = extension_upperCheckBox
 
         self.min_Label = min_Label
         self.max_Label = max_Label
         self.step_Label = step_Label
         self.ascending_Label = ascending_Label
 
         self.contour_levels_help = None  # No external window yet.
@@ -3498,16 +3693,28 @@
 
         # Set initial widget states
         self.level_type('automatic')
 
         self.show()
 
 
+    def level_management(self, text):
+        '''Set visibility of level management options'''
+       
+        if self.user_managementCheckBox.isChecked():
+            self.management_frame.show()
+        else:
+            self.management_frame.hide()
+           
+
+
+
+
     def level_type(self, text):
- 
+        '''Set the level types'''
         types = ['automatic', 'even', 'manual']
         vars = [plotvars.levs_automatic_set,  plotvars.levs_set, plotvars.levs_manual_set]
         checkboxes = [self.automaticCheckBox, self.evenCheckBox, self.manualCheckBox]
         state = [False, False, False]
         loc = types.index(text)
         state[loc] = True
 
@@ -3546,39 +3753,165 @@
             obj.setEnabled(flags[i])
             pal = QPalette(obj.palette())
             pal.setColor(QPalette.WindowText, QColor(color))
             obj.setPalette(pal)
 
 
     def levs_even_changed(self):
+        '''Change the even levels'''         
         plotvars.levs_min = self.levs_minTextbox.text()
         plotvars.levs_max = self.levs_maxTextbox.text()
         plotvars.levs_step = self.levs_stepTextbox.text()
 
 
     def levs_manual_changed(self):
+        '''Change the manual levels'''
         plotvars.levs_manual = self.levs_manualTextbox.text()
         
 
     def reset(self):
+        '''Reset eveything'''
         self.level_type('automatic')
         self.levs_minTextbox.setText('')
         self.levs_maxTextbox.setText('')
         self.levs_stepTextbox.setText('')
         self.levs_manualTextbox.setText('')
         plotvars.levs_set = False
         
         
     def extension_type(self, text):
+        '''Change the colour bar extension type'''
+        plotvars.levs_extend_lower = self.extension_lowerCheckBox.isChecked()
+        plotvars.levs_extend_upper = self.extension_upperCheckBox.isChecked()
+        
+        
+    def user_levels_changed(self, text):
+        '''Change the user interface settings based on the stored values for user levels '''
+        
+        mylevels = plotvars.levels_stored[text]
+        
+        
+        self.automaticCheckBox.setChecked(True)
+        self.evenCheckBox.setChecked(False)
+        self.manualCheckBox.setChecked(False)
+        self.levs_minTextbox.setText('')
+        self.levs_maxTextbox.setText('')
+        self.levs_stepTextbox.setText('')
+        self.levs_manualTextbox.setText('')
+        plotvars.levs_set = False
+        plotvars.levs_manual_set = False
+        plotvars.levs_min = ''
+        plotvars.levs_max = ''
+        plotvars.levs_step = ''
+        plotvars.levs_manual = ''
+        plotvars.levs_extend_lower = True
+        plotvars.levs_extend_upper = True
+
+        if text != 'default':
+            self.automaticCheckBox.setChecked(False)
+
+        if mylevels['min'] != '' or mylevels['max'] != '' or mylevels['step'] !='':
+            self.evenCheckBox.setChecked(True)
+            self.levs_minTextbox.setText(mylevels['min'])
+            self.levs_maxTextbox.setText(mylevels['max'])
+            self.levs_stepTextbox.setText(mylevels['step'])
+            plotvars.levs_set = True           
+            
+        if mylevels['manual'] != '':
+            self.manualCheckBox.setChecked(True)
+            self.levs_manualTextbox.setText(mylevels['manual'])
+            plotvars.levs_manual_set = True
+
+        self.extension_lowerCheckBox.setChecked(mylevels['extend_lower'])
+        self.extension_upperCheckBox.setChecked(mylevels['extend_upper'])
+        
+        plotvars.levs_min = mylevels['min']
+        plotvars.levs_max = mylevels['max']
+        plotvars.levs_step = mylevels['step']
+        plotvars.levs_manual = mylevels['manual']
+        plotvars.levs_extend_lower = mylevels['extend_lower']
+        plotvars.levs_extend_upper = mylevels['extend_upper']
+        
+        
+        
+    def save_levels(self):
+        ''' Add a new levels saved name based on the current settings '''
+
+        name = self.save_levelsTextBox.text()
+        if name == '':
+            print('Cannot save current levels to a blank name')
+            return
+
+        if name in plotvars.levels_stored:
+            print('Cannot save current levels to name: ' + name + ' as it already exists')
+            return
+
+
+        # Add the new levels dictionary to plotvars.levels_stored
+        mylevels = {}
+        mylevels[name] = {}
+        mylevels[name]['min'] = plotvars.levs_min
+        mylevels[name]['max'] = plotvars.levs_max
+        mylevels[name]['step'] = plotvars.levs_step
+        mylevels[name]['manual'] = plotvars.levs_manual
+        mylevels[name]['extend_lower'] = plotvars.levs_extend_lower
+        mylevels[name]['extend_upper'] = plotvars.levs_extend_upper
+        plotvars.levels_stored.update(mylevels)
+
+
+        # Add the new map name to user_mapsComboBox
+        self.user_levelsComboBox.addItem(name)
+        mylen = self.user_levelsComboBox.count()
+        self.user_levelsComboBox.setCurrentIndex(mylen-1)
+
+
+    def save_settings(self):
+        ''' Save the current map settings in the specified file.
+            Normally this would be ~/.cfview_defaults '''
+
+        # Ask whether to clobber an existing file
+        full_path = os.path.expanduser(self.save_settingsTextBox.text())
+        self.savefile = full_path
+        check = os.path.isfile(full_path)
+
+        if check:
+            html = ''
+            html += '<body>The file ' + full_path + ' already exists'
+            html += '<p>Okay to overwrite?</body>'
+
+
+            self.clobber = Clobber_file(html, self.savefile)
+
+            self.clobber.show()
+
+        else:
+            plotvars.write_defaults = True
+
+        Save_defaults(self.savefile)
+
+
+    def delete_levels(self):
+        ''' Delete the current highlighted levels '''
+
+        levels = self.user_levelsComboBox.currentText()
+
+        if map == 'default':
+           print('Cannot delete the default levels')
+           return
+
+        del(plotvars.levels_stored[levels])
+
+        index = self.user_levelsComboBox.currentIndex()
+        self.user_levelsComboBox.removeItem(index)
+        self.user_levelsComboBox.setCurrentIndex(0)
 
-        plotvars.levs_extend_lower = self.extension_lowerCheck.isChecked()
-        plotvars.levs_extend_upper = self.extension_upperCheck.isChecked()
 
 
     def help(self):
+        '''Help section for contour levels'''
         if self.contour_levels_help is None:
 
             html = ''
             html += '<body><h2>Contour level options</h2>'
             html += 'Contour levels are initially set automatically based on the range of the field and '
             html += 'split into reasonable contour levels. If a region of the field is chosen for contouring '
             html += 'then the range of the full field is still used.'
@@ -3586,21 +3919,28 @@
             html += '<h3>Setting contour levels</h3>'
             html += 'When making plots that compare data click on the evenly or manually spaced levels tick '
             html += 'boxes and set them as appropriate. Manualy spaced levels must be separated by spaces and ascend in value.'
 
             html += '<h3>Colorbar extensions</h3>'
             html += 'Colorbar extensions are a way of extending the contours to cover all the data at the ends of the '
             html += 'contour range. Click on the colorbar extension tick boxes as appropriate if these are both required.</p></body>' 
+            
+            html += "<h3>Contour level management</h3>"
+            html += "Options are:<br>"
+            html += "Saving the current contour level settings to the specified name.<br>"
+            html += "Saving all current contour level and cfview settings to a sepcified file.  Nominally "
+            html += "this is ~/.cfview_defaults<br>"
+            html += "Deleting the currently highlighted contour levels.  You cannot delete the default contour levels"
 
             self.contour_levels_help = Help(html)
 
         self.contour_levels_help.show()
 
     def closeEvent(self, event):
-        # Close self.parent.contour_levels_window
+        ''' Close self.parent.contour_levels_window '''
         self.parent.contour_levels_window = None
         self.close()
 
 
 
 
 
@@ -3613,15 +3953,16 @@
     def __init__(self, html):
         super(Help, self).__init__()
         self.html = html
         self.initUI()
 
 
     def initUI(self):
-
+        ''' Main window layout '''
+        
         quitButton = QPushButton("Quit")
         quitButton.clicked.connect(self.close)
 
 
         helpTextbox = QTextEdit()
         helpTextbox.setReadOnly(True)
 
@@ -3661,111 +4002,143 @@
         self.setMinimumSize(600, 600)
 
         self.show()
 
 
 
 class HLine(QFrame):
+    '''Horizontal line class'''
     def __init__(self, parent=None, color=QColor(plotvars.text_colour)):
 
         super(HLine, self).__init__(parent)
         self.setFrameShape(QFrame.HLine)
         self.setFrameShadow(QFrame.Plain)
         self.setFixedHeight(40)
         self.setLineWidth(0)
         self.setMidLineWidth(3)
         self.setContentsMargins(0, 0, 0, 0)
         self.setColor(color)
 
     def setColor(self, color):
+        '''Set the horizontal line colour'''
         pal = self.palette()
         pal.setColor(QPalette.WindowText, color)
         self.setPalette(pal)
 
 
 class Colour_scale_window(QWidget):
-    '''popup window for changing colour scale defaults'''
+    '''Popup window for changing colour scale defaults'''
 
     def __init__(self, parent):
         super(Colour_scale_window, self).__init__()
         
         self.parent = parent
         self.initUI()
 
 
     def initUI(self):
-
+        ''' Main window layout '''
+        
         # Set up some buttons
         resetButton = QPushButton("Reset")
         resetButton.clicked.connect(self.reset)
 
         helpButton = QPushButton("Help")
         helpButton.clicked.connect(self.help)
 
         quitButton = QPushButton("Quit")
         quitButton.clicked.connect(self.closeEvent)
-
+        
+        save_scaleButton = QPushButton('Save settings to this user scale name:')
+        save_scaleButton.clicked.connect(self.save_scale)
+        save_settingsButton = QPushButton('Save all cfview settings to this file:')
+        save_settingsButton.clicked.connect(self.save_settings)
+        delete_scaleButton = QPushButton('Delete currently selected user scale')
+        delete_scaleButton.clicked.connect(self.delete_scale)
+
+        # Set up user scales dropdown
+        user_scalesComboBox = QComboBox()
+        myscales = plotvars.scales_stored
+        for myscale in myscales:
+            user_scalesComboBox.addItem(myscale)
+        user_scalesComboBox.activated[str].connect(self.user_scale_changed)
+        self.user_scalesComboBox = user_scalesComboBox
 
 
         # Scale selection tick boxes
         automaticCheckBox = QCheckBox("Automatic colour scale")
         automaticCheckBox.setChecked(True)
         automaticCheckBox.clicked.connect(self.automatic)
 
         reverseCheckBox = QCheckBox("Reverse colour scale")
         reverseCheckBox.setChecked(False)
         reverseCheckBox.clicked.connect(self.reverse)
 
-        # Text box labels
+        # Labels
         numberLabel = QLabel('Number of colours in the scale')
         whiteLabel = QLabel('Set these indicies to be white')
-        aboveLabel = QLabel('Number of colours above the scale midpoint')
-        belowLabel = QLabel('Number of colours below the scale midpoint')
+        midpointLabel = QLabel('Number of colours:')
+        aboveLabel = QLabel('above scale midpoint')
+        belowLabel = QLabel('below scale midpoint')
+        user_scaleLabel = QLabel('User Scales:')
+
 
         pal = QPalette(numberLabel.palette())
         pal.setColor(QPalette.WindowText, QColor('#708090'))
         numberLabel.setPalette(pal)
 
         # Text boxes
         numberTextBox = QLineEdit()
         numberTextBox.textChanged.connect(lambda: self.text_changed('number'))
         whiteTextBox = QLineEdit()
         whiteTextBox.textChanged.connect(lambda: self.text_changed('white'))
         aboveTextBox = QLineEdit()
         aboveTextBox.textChanged.connect(lambda: self.text_changed('above'))
         belowTextBox = QLineEdit()
         belowTextBox.textChanged.connect(lambda: self.text_changed('below'))
+        save_scaleTextBox = QLineEdit()
+        save_settingsTextBox = QLineEdit()
+        save_settingsTextBox.setText('~/.cfview_defaults')
+
+        self.save_scaleTextBox = save_scaleTextBox
+        self.save_settingsTextBox = save_settingsTextBox
 
 
         # Set the layout
         vbox = QVBoxLayout()
+        
+        # User defined levels
+        hbox_cscales = QHBoxLayout()
+        hbox_cscales.addWidget(user_scaleLabel)
+        hbox_cscales.addWidget(user_scalesComboBox)
+        vbox.addLayout(hbox_cscales)
+
         hbox_number = QHBoxLayout()
         hbox_white = QHBoxLayout()
-        hbox_above = QHBoxLayout()
-        hbox_below = QHBoxLayout()
+        hbox_midpoint = QHBoxLayout()
+        #hbox_below = QHBoxLayout()
         hbox_buttons = QHBoxLayout()
 
         vbox.addWidget(automaticCheckBox)
         vbox.addWidget(HLine())
 
         vbox.addLayout(hbox_number)
         hbox_number.addWidget(numberLabel)
         hbox_number.addWidget(numberTextBox)
 
         vbox.addLayout(hbox_white)
         hbox_white.addWidget(whiteLabel)
         hbox_white.addWidget(whiteTextBox)
 
-        vbox.addLayout(hbox_above)
-        hbox_above.addWidget(aboveLabel)
-        hbox_above.addWidget(aboveTextBox)
-
-        vbox.addLayout(hbox_below)
-        hbox_below.addWidget(belowLabel)
-        hbox_below.addWidget(belowTextBox)
+        vbox.addLayout(hbox_midpoint)
+        hbox_midpoint.addWidget(midpointLabel)
+        hbox_midpoint.addWidget(aboveLabel)
+        hbox_midpoint.addWidget(aboveTextBox)
+        hbox_midpoint.addWidget(belowLabel)
+        hbox_midpoint.addWidget(belowTextBox)
 
         vbox.addWidget(reverseCheckBox)
 
         vbox.addWidget(HLine())
 
         # Make a scrollable area for the colour bars and check boxes
         vbox_scale = QVBoxLayout()
@@ -3779,14 +4152,15 @@
         self.automaticCheckBox = automaticCheckBox
         self.reverseCheckBox = reverseCheckBox
         self.numberTextBox = numberTextBox
         self.whiteTextBox = whiteTextBox
         self.aboveTextBox = aboveTextBox
         self.belowTextBox = belowTextBox
         self.numberLabel = numberLabel
+        self.midpointLabel = midpointLabel
         self.aboveLabel = aboveLabel
         self.belowLabel = belowLabel
         self.whiteLabel = whiteLabel
 
 
 
         # Add the colours scale checkboxes and colour scales
@@ -3853,38 +4227,87 @@
             qim = QImage(data, im.size[0], im.size[1], QImage.Format_ARGB32)
             pixmap = QPixmap.fromImage(qim)
             image.setPixmap(pixmap)
 
             formLayout.addRow(getattr(self, scale + 'CheckBox'), image)
 
 
-        #self.viridisCheckBox.setChecked(True)
 
         groupBox.setLayout(formLayout)
         #vbox_scale.setLayout(formLayout)
         scroll = QScrollArea()
         scroll.setWidget(groupBox)
         scroll.setWidgetResizable(True)
         scroll.setFixedHeight(400)
         vbox_scale.addWidget(scroll)
 
 
+        vbox.addWidget(HLine())
+
+        # Saving levels options
+        user_managementCheckBox = QCheckBox('View user scale management options')
+        user_managementCheckBox.clicked.connect(partial(self.scale_management, 'clicked'))
+        self.user_managementCheckBox = user_managementCheckBox        
+        vbox.addWidget(user_managementCheckBox)        
+        
+        # Put management options in a frame as this can be hidden whereas a QVBoxLayout cannot 
+        management_frame = QFrame()
+        
+        vbox2 = QVBoxLayout() 
+               
+        hbox_save_scale = QHBoxLayout()
+        hbox_save_scale.addWidget(save_scaleButton)
+        hbox_save_scale.addWidget(save_scaleTextBox)
+        vbox2.addLayout(hbox_save_scale)
+
+        hbox_save_settings = QHBoxLayout()
+        hbox_save_settings.addWidget(save_settingsButton)
+        hbox_save_settings.addWidget(save_settingsTextBox)
+        vbox2.addLayout(hbox_save_settings)
+
+        hbox_delete_scale = QHBoxLayout()
+        hbox_delete_scale.addWidget(delete_scaleButton)
+        hbox_delete_scale.addStretch(1)
+        vbox2.addLayout(hbox_delete_scale)
 
+        management_frame.setLayout(vbox2)
+        management_frame.hide()
+        self.management_frame = management_frame
+        vbox.addWidget(management_frame)
 
 
-        vbox.addLayout(hbox_buttons)
+
+        #vbox.addLayout(hbox_buttons)
         hbox_buttons.addWidget(resetButton)
         hbox_buttons.addWidget(helpButton)
         hbox_buttons.addWidget(quitButton)
 
+        # Make a scrollable area
+        groupBox = QGroupBox('')
+        groupBox.setLayout(vbox)
+        scroll = QScrollArea()
+        scroll.setWidget(groupBox)
+        scroll.setWidgetResizable(True)
+        vscroll = scroll.verticalScrollBar()
+        #scroll.setFixedWidth(800)
+        #scroll.setFixedHeight(800)
+        container = QVBoxLayout()
+        container.addWidget(scroll)
 
+        container.addLayout(hbox_buttons)
+        
+        self.scroll = scroll
+        self.vscroll = vscroll
+        self.setLayout(container)
+        
+        
         self.colour_scale_help = None  # No external window yet.
 
         self.setWindowTitle('cfview colour scales')
-        self.setLayout(vbox)
+        #self.setLayout(vbox)
 
 
 
         # Set theme and font
         palette = QPalette()
         palette.setColor(QPalette.Window, QColor(plotvars.background_colour))
         palette.setColor(QPalette.Base, QColor(plotvars.background_colour))
@@ -3903,97 +4326,206 @@
         plotvars.cscale_automatic_set = self.automaticCheckBox.isChecked()
         self.set_sensitive()
 
         self.show()
 
 
 
+
+    def scale_management(self, text):
+        '''Set visibility of scale management options'''
+       
+        if self.user_managementCheckBox.isChecked():
+            self.management_frame.show()
+        else:
+            self.management_frame.hide()
+
+
+
     def text_changed(self, textbox):
+        '''Change plotvars values when a textbox is changed'''
         if textbox == 'number':
             plotvars.cscale_ncols = self.numberTextBox.text()
         if textbox == 'white':
             plotvars.cscale_white = self.whiteTextBox.text()
         if textbox == 'above':
             plotvars.cscale_above = self.aboveTextBox.text()
         if textbox == 'below':
             plotvars.cscale_below = self.belowTextBox.text()
 
 
 
 
 
     def automatic(self):
-        # Toggle automatic colour scales
+        '''Toggle automatic colour scales'''
         if self.automaticCheckBox.isChecked():
             self.reset()
         else:
             plotvars.cscale_automatic_set = self.automaticCheckBox.isChecked()
             self.set_sensitive()
 
 
     def set_sensitive(self):
-        # Set the sensitivity and color of the widgets
+        '''Set the sensitivity and color of the widgets'''
 
         if plotvars.cscale_automatic_set:
             color = plotvars.text_colour_insensitive
             enabled = False
         else:
             color = plotvars.text_colour
             enabled = True
 
         objs = [self.reverseCheckBox, self.numberTextBox, self.whiteTextBox, self.aboveTextBox, \
                self.belowTextBox, self.reverseCheckBox, self.numberLabel, self.aboveLabel,\
-               self.belowLabel, self.whiteLabel]
+               self.belowLabel, self.midpointLabel, self.whiteLabel]
         for scale in plotvars.cscales:
             objs.append(getattr(self, scale + 'CheckBox'))
 
         for obj in objs:
             obj.setEnabled(enabled)
             pal = QPalette(obj.palette())
             pal.setColor(QPalette.WindowText, QColor(color))
             obj.setPalette(pal)
 
 
     def reverse(self):
-        plotvars.cscale_reverse_set = self.reverseCheckBox.isChecked()
+        '''Set colour scale reverse option'''
+        plotvars.cscale_reverse = self.reverseCheckBox.isChecked()
 
 
     def scale_changed(self, myscale):
+        '''Change the colour scale'''
         for scale in plotvars.cscales:
             getattr(self, scale + 'CheckBox').setChecked(False)
 
         getattr(self, myscale + 'CheckBox').setChecked(True)
         plotvars.cscale = myscale
 
 
-    def reset(self):
 
+    def user_scale_changed(self, text):
+        ''' Change the user interface settings based on the stored values for user scales '''
+
+        myscale = plotvars.scales_stored[text]
+
+        self.reset()
+        
+        if text != 'default':
+            self.automaticCheckBox.setChecked(False)
+            plotvars.cscale_automatic_set = False
+            self.reverseCheckBox.setChecked(myscale['reverse'])
+            self.numberTextBox.setText(myscale['ncols'])
+            self.whiteTextBox.setText(myscale['white'])
+            self.aboveTextBox.setText(myscale['above'])
+            self.belowTextBox.setText(myscale['below'])           
+            getattr(self, myscale['scale'] + 'CheckBox').setChecked(True)
+             
+            plotvars.cscale = myscale['scale']
+            plotvars.cscale_reverse = myscale['reverse']
+            plotvars.cscale_white = myscale['white']
+            plotvars.cscale_ncols = myscale['ncols']
+            plotvars.cscale_above = myscale['above']
+            plotvars.cscale_below =  myscale['below']
+
+
+    def save_scale(self):
+        ''' Add a new scale saved name based on the current settings '''
+
+        name = self.save_scaleTextBox.text()
+        if name == '':
+            print('Cannot save current scale to a blank name')
+            return
+
+        if name in plotvars.scales_stored:
+            print('Cannot save current scale to name: ' + name + ' as it already exists')
+            return
+
+
+        # Add the new scale dictionary to plotvars.scale_stored
+        myscale = {}
+        myscale[name] = {}
+        myscale[name]['ncols'] = plotvars.cscale_ncols
+        myscale[name]['white'] = plotvars.cscale_white
+        myscale[name]['reverse'] = plotvars.cscale_reverse
+        myscale[name]['above'] = plotvars.cscale_above
+        myscale[name]['below'] = plotvars.cscale_below
+        myscale[name]['scale'] = plotvars.cscale
+        plotvars.scales_stored.update(myscale)
+
+
+        # Add the new map name to user_mapsComboBox
+        self.user_scalesComboBox.addItem(name)
+        mylen = self.user_scalesComboBox.count()
+        self.user_scalesComboBox.setCurrentIndex(mylen-1)
+
+    def save_settings(self):
+        ''' Save the current map settings in the specified file.
+            Normally this would be ~/.cfview_defaults '''
+
+        # Ask whether to clobber an existing file
+        full_path = os.path.expanduser(self.save_settingsTextBox.text())
+        self.savefile = full_path
+        check = os.path.isfile(full_path)
+
+        if check:
+            html = ''
+            html += '<body>The file ' + full_path + ' already exists'
+            html += '<p>Okay to overwrite?</body>'
+
+
+            self.clobber = Clobber_file(html, self.savefile)
+
+            self.clobber.show()
+
+        else:
+            plotvars.write_defaults = True
+
+        Save_defaults(self.savefile)
+
+    def delete_scale(self):
+        ''' Delete the current highlighted user scale '''
+
+        scale = self.user_scaleComboBox.currentText()
+
+        if scale == 'default':
+           print('Cannot delete the default scale')
+           return
+
+        del(plotvars.scales_stored[scale])
+
+        index = self.user_scaleComboBox.currentIndex()
+        self.user_scaleComboBox.removeItem(index)
+        self.user_scaleComboBox.setCurrentIndex(0)
+
+
+    def reset(self):
+        '''Reset the colour scale options'''
         self.automaticCheckBox.setChecked(True)
         plotvars.cscale_automatic_set = True
         self.reverseCheckBox.setChecked(False)
         self.numberTextBox.setText('')
         self.whiteTextBox.setText('')
         self.aboveTextBox.setText('')
         self.belowTextBox.setText('')
         
         for scale in plotvars.cscales:
             getattr(self, scale + 'CheckBox').setChecked(False)
 
-        #self.viridisCheckBox.setChecked(True)
-        plotvars.cscale = 'viridis'
-        plotvars.cscale_reverse_set = False
+        plotvars.cscale = None
+        plotvars.cscale_reverse = False
         plotvars.cscale_white = ''
         plotvars.cscale_ncols = ''
         plotvars.cscale_above = ''
         plotvars.cscale_below = ''
         
         self.set_sensitive()
 
     def help(self):
-
+        '''Help for colour scale popup'''
         if self.colour_scale_help is None:
 
             html = ""
             html += "<body><h2>Colour scale options</h2>"
             html += "With the automatic colour scale option ticked cfview selects the colour scale depending "
             html += "on the data to be contoured:<p>"
             html += "viridis - fields that don\'t span zero - temperature in Kelvin etc.  This is a perceptually "
@@ -4005,103 +4537,148 @@
             html += "When a different colour scale is selected the scale will be automatically adjusted "
             html += "to fit the number of contour levels.<p>"
             html += "<h3>Selecting the number of colours</h3>"
             html += "Set the number of colours in the scale to gain more control over the colour scale. "
             html += "Once this is done then the white indicies and scale midpoint options become useful "
             html += "to allow more precise scale manipulation.  Set a number of white colour indicies by leaving "
             html += "a space between the indices required.<p>"
-
+            
+            html += "<h3>Colour scale management</h3>"
+            html += "Options are:<br>"
+            html += "Saving the current colour scale settings to the specified name.<br>"
+            html += "Saving all current colour scales and cfview settings to a sepcified file.  Nominally "
+            html += "this is ~/.cfview_defaults<br>"
+            html += "Deleting the currently highlighted colour scale.  You cannot delete the default colour scale"
             self.colour_scale_help = Help(html)
 
         self.colour_scale_help.show()
         
     def closeEvent(self, event):
-        # Close self.parent.colour_scale_window
+        '''Close self.parent.colour_scale_window'''
         self.parent.colour_scale_window = None
         self.close()
         
 
 
 class Map_window(QWidget):
-    '''popup window for changing map defaults'''
+    ''' Popup window for managing map defaults '''
 
     def __init__(self, parent):
         super(Map_window, self).__init__()
         
         self.parent = parent
         self.initUI()
 
 
     def initUI(self):
-
+        ''' Main window layout '''
+        
         # Set up some buttons
         resetButton = QPushButton("Reset")
         resetButton.clicked.connect(self.reset)
 
         helpButton = QPushButton("Help")
         helpButton.clicked.connect(self.help)
 
         quitButton = QPushButton("Quit")
         quitButton.clicked.connect(self.closeEvent)
-
+        
+        save_mapButton = QPushButton('Save settings to this map name:')
+        save_mapButton.clicked.connect(self.save_map)
+        save_settingsButton = QPushButton('Save all cfview settings to this file:')   
+        save_settingsButton.clicked.connect(self.save_settings)
+        delete_mapButton = QPushButton('Delete currently selected map')
+        delete_mapButton.clicked.connect(self.delete_map)
+             
 
         # Text box labels
         lonminLabel = QLabel('lonmin')
         lonmaxLabel = QLabel('lonmax')
         latminLabel = QLabel('latmin')
         latmaxLabel = QLabel('latmax')
         boundinglatLabel = QLabel('Bounding latitude')
         lon_0Label = QLabel('Longitude centre of map domain')
         other_map_typesLabel = QLabel('Other map types')
-        continent_attributesLabel = QLabel('Continent Attributes')
+        continent_attributesLabel = QLabel('Map Properties')
         continent_thicknessLabel = QLabel('Thickness')
         continent_colorLabel = QLabel('Colour')
+        resolutionLabel = QLabel('Resolution')
+        user_mapsLabel = QLabel('User map:')
 
+        
         # Text boxes
         lonminTextBox = QLineEdit()
-        lonminTextBox.setText('-180')
+        lonminTextBox.setText(str(plotvars.lonmin))
         lonminTextBox.textChanged.connect(lambda: self.textbox_changed('lonmin'))
         lonmaxTextBox = QLineEdit()
-        lonmaxTextBox.setText('180')
+        lonmaxTextBox.setText(str(plotvars.lonmax))
         lonmaxTextBox.textChanged.connect(lambda: self.textbox_changed('lonmax'))
         latminTextBox = QLineEdit()
-        latminTextBox.setText('-90')
+        latminTextBox.setText(str(plotvars.latmin))
         latminTextBox.textChanged.connect(lambda: self.textbox_changed('latmin'))
         latmaxTextBox = QLineEdit()
-        latmaxTextBox.setText('90')
+        latmaxTextBox.setText(str(plotvars.latmax))
         latmaxTextBox.textChanged.connect(lambda: self.textbox_changed('latmax'))
         boundinglatTextBox = QLineEdit()
-        boundinglatTextBox.setText('0')
+        boundinglatTextBox.setText(str(plotvars.boundinglat))
         boundinglatTextBox.textChanged.connect(lambda: self.textbox_changed('boundinglat'))
         lon_0TextBox = QLineEdit()
-        lon_0TextBox.setText('0')
+        lon_0TextBox.setText(str(plotvars.lon_0))
         lon_0TextBox.textChanged.connect(lambda: self.textbox_changed('lon_0'))
         continent_thicknessTextBox = QLineEdit()
-        continent_thicknessTextBox.setText('1.5')
+        continent_thicknessTextBox.setText(str(plotvars.continent_thickness))
         continent_thicknessTextBox.textChanged.connect(lambda: self.textbox_changed('continent_thickness'))
         continent_colorTextBox = QLineEdit()
-        continent_colorTextBox.setText('black')
+        continent_colorTextBox.setText(str(plotvars.continent_color))
         continent_colorTextBox.textChanged.connect(lambda: self.textbox_changed('continent_color'))
+        save_mapTextBox = QLineEdit()
+        save_settingsTextBox = QLineEdit()
+        save_settingsTextBox.setText('~/.cfview_defaults')
+
 
         # Map type check boxes
         maps = ['Cylindrical', 'EuroPP', 'LambertConformal', 'Mercator', 'Mollweide',\
                 'NorthPoleStereographic', 'Orthographic', 'OSGB', 'Robinson',\
                 'SouthPoleStereographic', 'UKCP', 'rotated']
         maps_short = ['cyl', 'EuroPP', 'lcc', 'merc', 'moll', 'npstere', 'ortho',\
                       'OSGB', 'robin', 'spstere', 'UKCP', 'rotated']
 
         for i in np.arange(len(maps)):
             setattr(self, maps[i] + 'CheckBox', QCheckBox(maps[i]))
             getattr(self, maps[i] + 'CheckBox').setChecked(False)
             getattr(self, maps[i] + 'CheckBox').clicked.connect(partial(self.map_type, maps_short[i]))
 
-        self.CylindricalCheckBox.setChecked(True)
-
-
-
+        myindex = maps_short.index(plotvars.proj)
+        getattr(self, maps[myindex] + 'CheckBox').setChecked(True)
+        
+        
+        # If the field is not a rotated one turn off the sensitivity of the rotated checkbox
+        if len(plotvars.fields) > 0:
+            obj = self.rotatedCheckBox
+            pal = QPalette(obj.palette())
+            
+            if plotvars.fields[plotvars.index_number].ref('grid_mapping_name:rotated_latitude_longitude', default=False):
+                obj.setEnabled(True)
+                pal.setColor(QPalette.WindowText, QColor(plotvars.text_colour))
+            else:
+                obj.setEnabled(False)
+                pal.setColor(QPalette.WindowText, QColor(plotvars.text_colour_insensitive))    
+                            
+            obj.setPalette(pal)                 
+        
+        
+        
+        # Set up user map dropdown     
+        user_mapsComboBox = QComboBox()
+        mymaps = plotvars.maps_stored
+        for mymap in mymaps:
+            user_mapsComboBox.addItem(mymap)
+        user_mapsComboBox.activated[str].connect(self.user_map_changed)
+        self.user_mapsComboBox = user_mapsComboBox
+        
 
         self.lonminLabel = lonminLabel
         self.lonmaxLabel = lonmaxLabel
         self.latminLabel = latminLabel
         self.latmaxLabel = latmaxLabel
         self.boundinglatLabel = boundinglatLabel
         self.lon_0Label = lon_0Label
@@ -4114,33 +4691,52 @@
         self.lonmaxTextBox = lonmaxTextBox
         self.latminTextBox = latminTextBox
         self.latmaxTextBox = latmaxTextBox
         self.boundinglatTextBox = boundinglatTextBox
         self.lon_0TextBox = lon_0TextBox
         self.continent_thicknessTextBox = continent_thicknessTextBox
         self.continent_colorTextBox = continent_colorTextBox
-
+        self.save_mapTextBox = save_mapTextBox
+        self.save_settingsTextBox = save_settingsTextBox
+        
+        user_managementCheckBox = QCheckBox('View user map management options')
+        user_managementCheckBox.clicked.connect(partial(self.map_management, 'clicked'))
+        self.user_managementCheckBox = user_managementCheckBox
+        
+        
         # Set the layout
         vbox = QVBoxLayout()
 
+        # User defined maps
+        hbox_maps = QHBoxLayout()
+        hbox_maps.addWidget(user_mapsLabel)
+        hbox_maps.addWidget(user_mapsComboBox)
+        vbox.addLayout(hbox_maps)                 
+
         # Cylindrical options
         vbox.addWidget(self.CylindricalCheckBox)
         hbox_lons = QHBoxLayout()
         hbox_lons.addWidget(self.lonminLabel)
         hbox_lons.addWidget(self.lonminTextBox)
         hbox_lons.addWidget(self.lonmaxLabel)
         hbox_lons.addWidget(self.lonmaxTextBox)
+        
+        hbox_lons.addWidget(self.latminLabel)
+        hbox_lons.addWidget(self.latminTextBox)
+        hbox_lons.addWidget(self.latmaxLabel)
+        hbox_lons.addWidget(self.latmaxTextBox)        
+        
         vbox.addLayout(hbox_lons)
 
-        hbox_lats = QHBoxLayout()
-        hbox_lats.addWidget(self.latminLabel)
-        hbox_lats.addWidget(self.latminTextBox)
-        hbox_lats.addWidget(self.latmaxLabel)
-        hbox_lats.addWidget(self.latmaxTextBox)
-        vbox.addLayout(hbox_lats)
+        #hbox_lats = QHBoxLayout()
+        #hbox_lats.addWidget(self.latminLabel)
+        #hbox_lats.addWidget(self.latminTextBox)
+        #hbox_lats.addWidget(self.latmaxLabel)
+        #hbox_lats.addWidget(self.latmaxTextBox)
+        #vbox.addLayout(hbox_lats)
 
         vbox.addWidget(HLine())
 
         # Polar options
         hbox_polar = QHBoxLayout()
         hbox_polar.addWidget(self.NorthPoleStereographicCheckBox)
         hbox_polar.addWidget(self.SouthPoleStereographicCheckBox)
@@ -4172,40 +4768,95 @@
         hbox_other2.addWidget(self.UKCPCheckBox)
         vbox.addLayout(hbox_other2)
         hbox_other3 = QHBoxLayout()
         hbox_other3.addWidget(self.rotatedCheckBox)
         vbox.addLayout(hbox_other3)
         vbox.addWidget(HLine())
 
-        # Continent thickness and colour
+        # Continent options
         vbox.addWidget(self.continent_attributesLabel)
-        hbox_thickness = QHBoxLayout()
-        hbox_thickness.addWidget(self.continent_thicknessLabel)
-        hbox_thickness.addWidget(self.continent_thicknessTextBox)
-        hbox_thickness.addStretch(1)
-        vbox.addLayout(hbox_thickness)
-        hbox_color = QHBoxLayout()
-        hbox_color.addWidget(self.continent_colorLabel)
-        hbox_color.addWidget(self.continent_colorTextBox)
-        hbox_color.addStretch(1)
-        vbox.addLayout(hbox_color)
-
+        #hbox_resolution = QHBoxLayout()        
+        resolutionComboBox = QComboBox()
+        resolutionComboBox.addItem('110m')
+        resolutionComboBox.addItem('50m')
+        resolutionComboBox.addItem('10m')
+        resolutionComboBox.activated[str].connect(self.resolution_changed)
+        self.resolutionComboBox = resolutionComboBox
+        self.resolutionComboBox.setCurrentText(plotvars.resolution)
+        
+        hbox_map = QHBoxLayout()  
+        hbox_map.addWidget(resolutionLabel)
+        hbox_map.addWidget(resolutionComboBox)
+        hbox_map.addWidget(self.continent_thicknessLabel)      
+        hbox_map.addWidget(self.continent_thicknessTextBox)     
+        hbox_map.addWidget(self.continent_colorLabel)   
+        hbox_map.addWidget(self.continent_colorTextBox)
+        vbox.addLayout(hbox_map)        
+        vbox.addWidget(HLine())
+        
+        # User map management
+        vbox.addWidget(user_managementCheckBox)
+        
+        # Put management options in a frame as this can be hidden whereas a QVBoxLayout cannot 
+        management_frame = QFrame()
+        
+        vbox2 = QVBoxLayout()
+        
+        hbox_save_map = QHBoxLayout()
+        hbox_save_map.addWidget(save_mapButton)
+        hbox_save_map.addWidget(save_mapTextBox)
+        vbox2.addLayout(hbox_save_map)
+        
+        hbox_save_settings = QHBoxLayout()
+        hbox_save_settings.addWidget(save_settingsButton)
+        hbox_save_settings.addWidget(save_settingsTextBox)
+        vbox2.addLayout(hbox_save_settings)       
+        
+        hbox_delete_map = QHBoxLayout()
+        hbox_delete_map.addWidget(delete_mapButton)
+        hbox_delete_map.addStretch(1)
+        vbox2.addLayout(hbox_delete_map)        
+        
 
-        # The buttons
+        management_frame.setLayout(vbox2)
+        management_frame.hide()
+        self.management_frame = management_frame
+        vbox.addWidget(management_frame)
+        
+        
+        
+        # The buttons at the bottom
         hbox_buttons = QHBoxLayout()
-        vbox.addLayout(hbox_buttons)
         hbox_buttons.addWidget(resetButton)
         hbox_buttons.addWidget(helpButton)
         hbox_buttons.addWidget(quitButton)
 
 
+
+        # Make a scrollable area
+        groupBox = QGroupBox('')
+        groupBox.setLayout(vbox)
+        scroll = QScrollArea()
+        scroll.setWidget(groupBox)
+        scroll.setWidgetResizable(True)
+        vscroll = scroll.verticalScrollBar()
+        #scroll.setFixedWidth(600)
+        #scroll.setFixedHeight(600)
+        container = QVBoxLayout()
+        container.addWidget(scroll)
+
+        container.addLayout(hbox_buttons)
+        
+        self.scroll = scroll
+        self.vscroll = vscroll
+        self.setLayout(container)
+
         self.map_help = None  # No external window yet.
 
         self.setWindowTitle('cfview map settings')
-        self.setLayout(vbox)
 
         # Set theme and font
         palette = QPalette()
         palette.setColor(QPalette.Window, QColor(plotvars.background_colour))
         palette.setColor(QPalette.Base, QColor(plotvars.background_colour))
         palette.setColor(QPalette.Button, QColor(plotvars.button_colour))
         palette.setColor(QPalette.ButtonText, QColor(plotvars.buttontext_colour))
@@ -4219,17 +4870,25 @@
         self.window().setFont(custom_font)
 
         # Set sensitivity of widgets
         self.set_sensitive()
 
         self.show()
 
+    def map_management(self, text):
+       '''Set visibility of map management options'''
+       
+       if self.user_managementCheckBox.isChecked():
+           self.management_frame.show()
+       else:
+           self.management_frame.hide()
+
 
     def map_type(self, text):
-
+        ''' Set the map type '''
         maps = ['Cylindrical', 'EuroPP', 'LambertConformal', 'Mercator', 'Mollweide',\
                 'NorthPoleStereographic', 'Orthographic', 'OSGB', 'Robinson',\
                 'SouthPoleStereographic', 'UKCP', 'rotated']
         maps_short = ['cyl', 'EuroPP', 'lcc', 'merc', 'moll', 'npstere', 'ortho', 'OSGB', 
                       'robin', 'spstere', 'UKCP', 'rotated']
 
 
@@ -4242,74 +4901,199 @@
         
         plotvars.proj = text
 
         self.set_sensitive()
 
 
     def textbox_changed(self, text):
-
+        ''' Set plotvars variables based on what is typed into the text boxes '''
         textbox = getattr(self, text + 'TextBox') 
         setattr(plotvars, text, textbox.text()) 
 
+    def resolution_changed(self, text):
+        ''' Change the map resolution '''
+        plotvars.resolution = text
+        
+        
+    def user_map_changed(self, text):
+        ''' Change the user interface settings based on the stored values for a user map '''
+        mymap = plotvars.maps_stored[text] 
+        
+        cfp.mapset()
+        cfp.setvars()
+        
+        # Set the text box values
+        for var in ['lonmin', 'lonmax', 'latmin', 'latmax', 'boundinglat', \
+                    'lon_0', 'continent_thickness', 'continent_color']:
+        
+            setattr(plotvars, var, mymap[var])
+            getattr(self, var + 'TextBox').setText(mymap[var])
+              
+        # Set the map tick boxes
+        maps = ['Cylindrical', 'EuroPP', 'LambertConformal', 'Mercator', 'Mollweide',\
+                'NorthPoleStereographic', 'Orthographic', 'OSGB', 'Robinson',\
+                'SouthPoleStereographic', 'UKCP', 'rotated']
+        maps_short = ['cyl', 'EuroPP', 'lcc', 'merc', 'moll', 'npstere', 'ortho', 'OSGB', 
+                      'robin', 'spstere', 'UKCP', 'rotated']
+                      
+        for i in np.arange(len(maps)):
+            getattr(self, maps[i] + 'CheckBox').setChecked(False)    
 
-    def set_sensitive(self):
-        # Set sensivity and colour of map widgets
+        index = maps_short.index(mymap['proj'])                      
+        getattr(self, maps[index] + 'CheckBox').setChecked(True)    
+        plotvars.proj = mymap['proj']
+        
+        # Set the resolution drop down
+        resolutions = ['110m', '50m', '10m']
+        res_index = resolutions.index(mymap['resolution'])
+        self.resolutionComboBox.setCurrentIndex(res_index)
+            
+        plotvars.resolution = mymap['resolution']
+            
+            
+    def save_map(self):
+        ''' Add a new map name based on the current settings '''
+        
+        name = self.save_mapTextBox.text()
+        if name == '':
+            print('Cannot save a map to a blank name')
+            return
+            
+        if name in plotvars.maps_stored:
+            print('Cannot save a map to name: ' + name + ' as it already exists')
+            return
+            
+
+        # Add the new map dictionary to plotvars.maps_stored
+        mymap = {}
+        mymap[name] = {}
+        mymap[name]['lonmin'] = plotvars.lonmin
+        mymap[name]['lonmax'] = plotvars.lonmax
+        mymap[name]['latmin'] = plotvars.latmin
+        mymap[name]['latmax'] = plotvars.latmax
+        mymap[name]['proj'] = plotvars.proj
+        mymap[name]['boundinglat'] = plotvars.boundinglat
+        mymap[name]['lon_0'] = plotvars.lon_0
+        mymap[name]['resolution'] = plotvars.resolution
+        mymap[name]['continent_thickness'] = plotvars.continent_thickness
+        mymap[name]['continent_color'] = plotvars.continent_color
+        plotvars.maps_stored.update(mymap)
+        
+               
+        # Add the new map name to user_mapsComboBox
+        self.user_mapsComboBox.addItem(name)
+        mylen = self.user_mapsComboBox.count()
+        self.user_mapsComboBox.setCurrentIndex(mylen-1)
+        
+        
+    def save_settings(self):
+        ''' Save the current map settings in the specified file.
+            Normally this would be ~/.cfview_defaults '''
+        
+        # Ask whether to clobber an existing file
+        full_path = os.path.expanduser(self.save_settingsTextBox.text())
+        self.savefile = full_path
+        check = os.path.isfile(full_path) 
+        
+        if check:
+            html = ''
+            html += '<body>The file ' + full_path + ' already exists'
+            html += '<p>Okay to overwrite?</body>'
+
+
+            self.clobber = Clobber_file(html, self.savefile)
+
+            self.clobber.show()
 
-        objs = [self.lonminLabel, self.lonminTextBox, self.lonmaxLabel,\
-                self.lonmaxTextBox, self.latminLabel, self.latminTextBox,\
-                self.latmaxLabel, self.latmaxTextBox,\
-                self.boundinglatLabel,\
-                self.boundinglatTextBox, self.lon_0Label, self.lon_0TextBox]
-
-        colors = [plotvars.text_colour] * 12
-        enabled = [False] * 12
-
-        if plotvars.proj in ['cyl', 'EuroPP', 'lcc', 'merc', 'ortho', 'OSGB',\
-                             'robin', 'UKCP']:
-            enabled[0:8] = [True] * 8
-            colors[8:] = [plotvars.text_colour_insensitive] * 4
         else:
-            colors[0:8] = [plotvars.text_colour_insensitive] * 8
-            enabled[8:] = [True] * 4
+            plotvars.write_defaults = True
+            
+        Save_defaults(self.savefile)
+        
+        
+              
+    def delete_map(self):
+        ''' Delete the current highlighted  map '''
+        
+        map = self.user_mapsComboBox.currentText()
+
+        if map == 'default':
+           print('Cannot delete the default map')
+           return
+
+        del(plotvars.maps_stored[map])
+
+        index = self.user_mapsComboBox.currentIndex()
+        self.user_mapsComboBox.removeItem(index)
+        self.user_mapsComboBox.setCurrentIndex(0)
+
 
+
+    def set_sensitive(self):
+        ''' Set the sensitivity and colour of map widgets '''
+
+        enabled = False
+        color = plotvars.text_colour_insensitive
+        if plotvars.proj in ['npstere', 'spstere']:
+            enabled = True
+            color = plotvars.text_colour
+            
+        objs = [self.boundinglatLabel, self.boundinglatTextBox, \
+                self.lon_0Label, self.lon_0TextBox]
+            
+            
         for i in np.arange(len(objs)):
             obj = objs[i]
-            obj.setEnabled(enabled[i])
+            obj.setEnabled(enabled)
             pal = QPalette(obj.palette())
-            pal.setColor(QPalette.WindowText, QColor(colors[i]))
-            obj.setPalette(pal)
-
+            pal.setColor(QPalette.WindowText, QColor(color))
+            obj.setPalette(pal)            
+            
+        
 
     def reset(self):
+        ''' Reset the map settings to the default '''
+        
         plotvars.proj = 'cyl'
         maps = ['Cylindrical', 'EuroPP', 'LambertConformal', 'Mercator', 'Mollweide',\
                 'NorthPoleStereographic', 'Orthographic', 'OSGB', 'Robinson',\
                 'SouthPoleStereographic', 'UKCP', 'rotated']
         for i in np.arange(len(maps)):
             getattr(self, maps[i] + 'CheckBox').setChecked(False)
 
         self.CylindricalCheckBox.setChecked(True)
         self.set_sensitive()
 
         self.lonminTextBox.setText('-180')
         self.lonmaxTextBox.setText('180')
         self.latminTextBox.setText('-90')
         self.latmaxTextBox.setText('90')
-        
-        plotvars.boundinglat = 0
-        plotvars.lon_0 = 0
         self.boundinglatTextBox.setText('0')
         self.lon_0TextBox.setText('0')
+        self.resolutionComboBox.setCurrentIndex(0)
         self.continent_thicknessTextBox.setText('1.5')
         self.continent_colorTextBox.setText('black')
 
+        plotvars.lonmin = '-180'
+        plotvars.lonmax = '180'
+        plotvars.latmin = '-90'
+        plotvars.latmax = '90'
+        plotvars.proj = 'cyl'
+        plotvars.lon_0 = '0'
+        plotvars.boundinglat = '0'
+        plotvars.continent_thickness = '1.5'
+        plotvars.continent_color = 'black'
+        plotvars.resolution = '110m'
+
         cfp.mapset()
+        cfp.setvars()
 
-    def help(self):
 
+    def help(self):
+        ''' Help text for map_window '''
         if self.map_help is None:
 
             html = ""
             html += "<body><h2>Map options</h2>"
             html += "<h3>Cylindrical projection</h3>"
             html += "The default map projection is the cylindrical equidistant projection with "
             html += "the limits of -180 to 180 degrees in longitude and -90 to 90 degrees in "
@@ -4319,48 +5103,55 @@
             html += "Polar plots are focussed on either the north or south pole. The bounding "
             html += "latitude is the edge of the viewable latitudes and is set to the equator "
             html += "by default. The centre of the map domain is where the map is centred. By "
             html += "default this is 0 degrees which is the Greenwich meridian in the case of "
             html += "the north pole. For the South Pole plot this is usually changed to 180 "
             html += "degrees."
             html += "<h3>Map resolution</h3>"
-            html += "The map resolution is set to a default of 110m. Higher resolutions such as "
-            html += "50m and 10m take more time to plot.  50m means 1:50,000,000 and not 50 metre."
+            html += "The map resolution is set to a default of 110m which is coarse. Higher resolutions such as "
+            html += "50m (medium) and 10m (fine) take more time to plot.  50m means 1:50,000,000 and not 50 metre."
 
-            html += "<h3>Continent color and thickness</h3>"
+            html += "<h3>Continent color, thickness and resolution</h3>"
             html += "These default to 1.5 and black. Matplotlib "
             html += "named colors can be seen using the following Python code at the Python "
-            html += "command prompt:<p>"
-
+            html += "command prompt:<br>"
             html += "<b>import matplotlib<br>"
             html += "for name in matplotlib.colors.cnames: print(name)</b>"
+            
+            html += "<h3>Map management</h3>"
+            html += "Options are:<br>"
+            html += "Saving the current map settings to the specified name.<br>"
+            html += "Saving all current maps and cfview settings to a sepcified file.  Nominally "
+            html += "this is ~/.cfview_defaults<br>"
+            html += "Deleting the currently highlighted map.  You cannot delete the default map"
 
             self.map_help = Help(html)
 
         self.map_help.show()
         
         
     def closeEvent(self, event):
-        # Close self.parent.colour_scale_window
+        ''' Close self.parent.colour_scale_window '''
         self.parent.colour_scale_window = None
         self.close()
 
 
 class Contour_window(QWidget):
-    '''popup window for changing contour defaults'''
+    '''Popup window for changing contour defaults'''
 
     def __init__(self, parent):
         super(Contour_window, self).__init__()
         
         self.parent = parent
         self.initUI()
 
 
     def initUI(self):
-
+        ''' Main window layout '''
+        
         # Set up some buttons
         resetButton = QPushButton("Reset")
         resetButton.clicked.connect(self.reset)
 
         helpButton = QPushButton("Help")
         helpButton.clicked.connect(self.help)
 
@@ -4467,14 +5258,16 @@
         self.window().setFont(custom_font)
 
 
         self.show()
 
 
     def contour_type(self, text):
+        ''' Set options in plotvars when the interface is changed '''
+        
         cbox = getattr(self, text + 'CheckBox')
         val = cbox.isChecked()
 
         if text == 'fill' and val:
             plotvars.blockfill = False
             plotvars.blockfill_fast = False
             self.blockfillCheckBox.setChecked(False)
@@ -4522,15 +5315,14 @@
             color = plotvars.text_colour_insensitive
             enabled = False
             
         if self.titlesCheckBox.isChecked():
             plotvars.titles = True
         else:
             plotvars.titles = False
-        print('plotvars.titles is ', plotvars.titles)
             
             
             
 
         objs = [self.automaticCheckBox, self.horizontalCheckBox, self.verticalCheckBox]
         for obj in objs:
             obj.setEnabled(enabled)
@@ -4539,15 +5331,16 @@
             obj.setPalette(pal)
 
 
         setattr(plotvars, text, val) 
 
 
     def reset(self):
-        # reset contour options
+        '''Reset contour options '''
+        
         self.fillCheckBox.setChecked(True)
         self.blockfillCheckBox.setChecked(False)
         self.blockfill_fastCheckBox.setChecked(False)
         self.linesCheckBox.setChecked(False)
         self.line_labelsCheckBox.setChecked(False)
         self.titleTextBox.setText('')
         self.nlevsTextBox.setText('')
@@ -4564,21 +5357,23 @@
         plotvars.line_labels = False
         plotvars.text = ''
         plotvars.colorbar_orientation = None
         plotvars.nlevs = False
         plotvars.titles = True
 
     def textbox_changed(self, text):
-
+        '''Set plotvars contour options based on textbox input'''
+        
         textbox = getattr(self, text + 'TextBox') 
         setattr(plotvars, text, textbox.text())         
         
         
     def help(self):
-
+        '''Help for contour options'''
+        
         if self.contour_help is None:
 
             html = '<body><h2>Contour options</h2>'
             html += 'Contour options of fill and blockfill are mutually exclusive.  If a '
             html += 'grid with lots of points in x and y is plotted then the blockfill '
             html += 'grid will not be readily visible until the plot is zoomed in<p>'
             html += 'blockfill_fast uses the matplotlib pcolormesh blockfill method which can produce '
@@ -4588,36 +5383,38 @@
             html += 'Finer contour level selection is available in the Setup -> contour levels pop up window.<p>'
             self.contour_help = Help(html)
 
         self.contour_help.show()
 
 
     def closeEvent(self, event):
-        # Close self.parent.contour_window
+        ''' Close self.parent.contour_window '''
+        
         self.parent.contour_window = None
         self.close()
 
 
 
 class TableModel(QAbstractTableModel):
-
+    ''' Add new definitions to TableModel '''
+    
     def __init__(self, data, x, y, ndecs, datamin, datamax, datamin_colour, datamax_colour):
         super(TableModel, self).__init__()
         self._data = data
         self._x = x
         self._y = y
         self._ndecs = ndecs
         self._datamin = datamin
         self._datamax = datamax
         self._datamin_colour = datamin_colour
         self._datamax_colour = datamax_colour
 
 
     def data(self, index, role): 
-
+        ''' Add colour and rounding to the data '''
 
         # Align table text to the right
         #if role == Qt.TextAlignmentRole and index.column() > 1:
         #     https://stackoverflow.com/questions/38150196/how-to-align-column-of-qtableview
         #     print('index.column to right' + str(index.column()))
         #     return Qt.AlignRight
         #return super(TableModel, self).data(index, role)
@@ -4647,21 +5444,26 @@
             if self._ndecs == 0:
                 return str(int(value))
             else:
                 return str(round(value, self._ndecs))
                  
 
     def rowCount(self, index):
+        '''Row count'''
+        
         return self._data.shape[0]
 
     def columnCount(self, index):
+        '''Column count'''
+        
         return self._data.shape[1]
 
     def headerData(self, section, orientation, role):
-
+        '''xlabels and ylabels for the data'''
+        
         if role != Qt.DisplayRole:
             return QVariant()
 
         if orientation == Qt.Horizontal:
             xlabels = []
             for ix in np.arange(len(self._x)):
                 xlabels.append(str(self._x[ix]))
@@ -4673,23 +5475,24 @@
                 ylabels.append(str(self._y[iy]))
             return ylabels[section]
     
 
 
 
 class Data_window(QWidget):
-    '''popup window for viewing data'''
+    '''Popup window for viewing data'''
 
     def __init__(self, parent):
         super(Data_window, self).__init__()
         self.parent = parent
         self.initUI()
 
     def initUI(self):
-
+        '''Main window layout'''
+        
         # Set up some buttons
         resetButton = QPushButton("Reset")
         resetButton.clicked.connect(self.reset)
 
         plotButton = QPushButton("Plot selected cells")
         plotButton.clicked.connect(self.plot)
 
@@ -4903,17 +5706,21 @@
         self.window().setFont(custom_font)
 
 
         self.show()
 
 
     def view_changed(self, value):
+        '''If the view changes call Populate_table'''
+        
         Populate_table(self)
 
     def plot(self):
+        '''Make a plot based on the selected data'''
+        
         selected = self.table.selectionModel().selectedIndexes()
 
         if selected:
             con_args ={}
             xvals = []
             yvals = []
             for item in selected:
@@ -5006,40 +5813,40 @@
 
 
 
 
 
 
     def reset(self):
-        # Reset data viewing values
+        '''Reset data viewing values'''
 
         self.ndecsSlider.setValue(2)
         self.column_widthSlider.setValue(10)
         self.column_widthLabel.setText('Column width: 10')
         self.text_sizeSlider.setValue(plotvars.fontsize)
         self.datamin_colourTextBox.setText('blue')
         self.datamax_colourTextBox.setText('red')
         self.dataminTextBox.setText('')
         self.datamaxTextBox.setText('')
         self.data_ComboBox.setCurrentIndex(0)
 
 
 
     def set_column_width(self, text):
-        # Set column width
+        '''Set column width'''
         
         width = self.column_widthSlider.value()
         self.column_widthLabel.setText('Column width: ' + str(width))
         self.width = width
         for i in np.arange(len(self.x)):
             self.table.setColumnWidth(i, width*10)
 
 
     def value_changed(self, text):
-        # reset the table based on the text boxes and ndecs slider
+        '''Reset the table based on the text boxes and ndecs slider'''
 
         datamin = self.dataminTextBox.text()
         datamax = self.datamaxTextBox.text()
         datamin_colour = self.datamin_colourTextBox.text()
         datamax_colour = self.datamax_colourTextBox.text()
 
         ndecs = int(self.ndecsSlider.value())
@@ -5056,15 +5863,16 @@
         self.table.setFont(custom_font)
 
 
         
 
 
     def help(self):
-
+        '''Help for data viewing popup'''
+        
         if self.data_help is None:
 
             html = ""
             html += "<body><h2>Data viewing</h2>"
             html += "Data viewing is based on the dimensions specied in the contour plot type with the default being x-y.  "
             html += "The field name, selected dimensions and plot type are displayed above the table of data."
             html += "Options to select the number of decimal places, text size and column width are provided to allow "
@@ -5074,15 +5882,15 @@
 
             self.data_help = Help(html)
 
         self.data_help.show()
 
 
     def closeEvent(self, event):
-        # Close self.parent.data_window
+        '''Close self.parent.data_window'''
         self.parent.data_window = None
         self.close()
 
 
 
 
 class Populate_table():
@@ -5092,15 +5900,16 @@
         super(Populate_table, self).__init__()
         self.parent = parent
         self.initial = initial
         self.change_table()
         
         
     def change_table(self):
-   
+        '''Change the table based on the widget values'''
+        
         # Set the field
         f = deepcopy(plotvars.fields[plotvars.index_number])
 
         
         mytypes = self.parent.data_ComboBox.currentText().split('-')
         if len(mytypes) == 2:
             myx = mytypes[0]
@@ -5239,24 +6048,25 @@
         self.parent.data = data
         self.parent.x = x
         self.parent.y = y
 
 
 
 class Names_window(QWidget):
-    '''popup window for changing data name defaults'''
+    '''Popup window for changing data name defaults'''
 
     def __init__(self, parent):
         super(Names_window, self).__init__()
         self.parent = parent
         self.initUI()
 
 
     def initUI(self):
-
+        '''Main window layout'''
+        
         # Set up some buttons
         saveButton = QPushButton("Save")
         saveButton.clicked.connect(self.save)
 
         new_propertyButton = QPushButton("New property")
         new_propertyButton.clicked.connect(self.new_property)
         
@@ -5343,15 +6153,15 @@
 
 
 
 
 
 
     def save(self):
-        # Save field if any changes have been made
+        '''Save field if any changes have been made'''
 
         # Initial check for change to vars that require a data reload
         reload = False
         data_changed = False
         for var in self.vardict:
             
             vals = self.vardict[var]
@@ -5514,23 +6324,23 @@
         
         
         
         
         
 
     def new_property(self):
-        # Pop-up for a new property 
+        '''Popup for a new property''' 
 
         if self.new_property_window is None:
             self.new_property_window = New_property_window(self)
             self.new_property_window.show()
  
         
     def reset(self):
-        # Reset the main Name window based on the field
+        '''Reset the main Name window based on the field'''
         
         # Delete all widgets in self.vbox_names
         if self.vbox_names.count() > 2:
             # Delete each widget in the layout one by one
             # We only have labels and hboxes
             while self.vbox_names.count():
                 item = self.vbox_names.takeAt(0)
@@ -5545,15 +6355,16 @@
                     for i in reversed(range(item.count())):
                         item_hbox = item.itemAt(i)
                         item_hbox.widget().setParent(None)
         
         Populate_names(self, initial=True)
 
     def help(self):
-
+        '''Help for the properties popup'''
+        
         if self.names_help is None:
 
             html = "<body><h2>Properties</h2>"
             html += "This window shows the properties for the field and dimensions as "
             html += "editable values.  Properties can also be deleted by pressing the 'X' button "
             html += "next to the property.  Changes to the in memory data are only made when the 'Save' "
             html += "button is pressed.  When the 'Reset' button is pressed the values will revert to "
@@ -5563,15 +6374,15 @@
 
             self.names_help = Help(html)
 
         self.names_help.show()
 
 
     def textbox_changed(self, text):
-        ''' Set value based on any text box change'''
+        '''Set value based on any text box change'''
 
         if text[:5] == 'field':
             var = 'field.' + text[5:]
 
         if text[:19] == 'dimensioncoordinate':
             var = "coord.('" + text[:20] + "')." + text[20:]
         
@@ -5583,15 +6394,15 @@
         self.vardict[var][3] = 'C'    
 
 
         
 
 
     def delete(self, text):
-
+        '''Delete a property'''
         name = None
 
         if text.split(' ')[0] in ['X', 'Y', 'Z', 'T']:
            name = "coord.('" + text[0] + "')." + text[2:] 
             
         if text[: 19] == 'dimensioncoordinate':
             name = "coord.('" + text[:20] + "')." + text[21:] 
@@ -5632,15 +6443,15 @@
 
         # Populate the window with the changed field names
         Populate_names(self, initial=False)
         
 
         
     def closeEvent(self, event):
-        # Close self.parent.names_window
+        '''Close self.parent.names_window'''
         self.parent.names_window = None
         self.close()
         
         
 
 class Populate_names():
     '''Populate names into the name viewing widget'''
@@ -5649,15 +6460,16 @@
         super(Populate_names, self).__init__()
         self.parent = parent
         self.initial = initial
         self.add_names()
         
         
     def add_names(self):
-   
+        '''Add the names based on the selected field'''
+        
         # Set the field
         field = plotvars.fields[plotvars.index_number]
 
         if self.initial:
         
             # Dictionary of names
             # vardict has the following variables:
@@ -5915,33 +6727,32 @@
     def __init__(self, parent):
         super(New_property_window, self).__init__()
         self.parent = parent
         self.initUI()
 
 
     def initUI(self):
-
+        '''Main window layout'''
+        
         applyButton = QPushButton("Apply")
         applyButton.clicked.connect(self.apply)
         helpButton = QPushButton("Help")
         helpButton.clicked.connect(self.help)
         quitButton = QPushButton("Quit")
         quitButton.clicked.connect(self.closeEvent)
         
-        dims = Cf_funcs.find_all_dims()
-        
+  
         # Make radio buttons
+        dims = plotvars.stored['f' + str(plotvars.index_number)]['data_axes']        
         rbuttons = ['field']
         for dim in dims:
-            if len(dim) == 1:
-                rbuttons.append(dim.lower())
-            else:
-                rbuttons.append(dim[:3] + dim[19:])
+            rbuttons.append(dim)
+        
 
-        # Make the radiobutons
+        # Add the radiobutons
         radiobuttons = []
         for rbutton in rbuttons:
             setattr(self, rbutton + 'RadioButton', QRadioButton(rbutton))
             getattr(self, rbutton + 'RadioButton').clicked.connect(partial(self.button_changed, rbutton))
             radiobuttons.append(getattr(self, rbutton + 'RadioButton'))
         self.radiobuttons = radiobuttons
 
@@ -5996,21 +6807,21 @@
         palette.setColor(QPalette.WindowText, QColor(plotvars.windowtext_colour))
         self.setPalette(palette)
 
         # Set font 
         custom_font = QFont(plotvars.font, plotvars.fontsize)
         self.window().setFont(custom_font)
 
-        self.setFixedWidth(600)
+        #self.setFixedWidth(600)
         self.setWindowTitle('cfview - create new properties')
 
         self.show()
 
     def apply(self):
-
+        '''Apply changes'''
         name = self.nameTextbox.text()
         if len(name) == 1:
             name = 'dimension ' + name
 
         val = Data_check.test_type(self.valueTextbox.text())
         
         if name == '':
@@ -6048,53 +6859,53 @@
 
 
         # Populate the window with the changed field names
         Populate_names(self.parent, initial=False)
 
 
     def button_changed(self, text):
-         
+        'Change variable name'''
         self.varname = text       
 
 
 
     def help(self):
-
+        '''Help for new property'''
         if self.new_property_help is None:
 
             html = '<body><h2>Add a new field property</h2>'
             html += 'Add a new property and value for the field, dimension or auxiliary coordinate'
 
-
             self.new_property_help = Help(html)
 
         self.new_property_help.show()
 
 
     def closeEvent(self, event):
-        # Close new_property window
+        '''Close new_property window'''
         self.parent.new_property_window = None
         self.close()
         
 
 
 
 
 class Transform_window(QWidget):
-    '''popup window for transforming data'''
+    '''Popup window for transforming data'''
 
 
     def __init__(self, parent):
         super(Transform_window, self).__init__()
         self.parent = parent
         self.initUI()
 
 
     def initUI(self):
-
+        '''Main window layout'''
+        
         # Set the layout
         vbox = QVBoxLayout()
         vbox_transform = QVBoxLayout()
         vbox.addLayout(vbox_transform)
         self.vbox = vbox
         self.vbox_transform = vbox_transform
         
@@ -6254,14 +7065,15 @@
         
         # Set the layout
 
         # Collapse methods
         vbox.addWidget(collapseLabel)
         hbox_area_collapse = QHBoxLayout()
         hbox_area_collapse.addWidget(self.collapse_areaLabel)
+        
         hbox_area_collapse.addWidget(self.collapse_areaComboBox)
         vbox.addLayout(hbox_area_collapse)
         
         for i in np.arange(plotvars.max_axes):
             hbox_collapse = QHBoxLayout()
             hbox_collapse.addWidget(self.collapse_Labels[i])
             hbox_collapse.addWidget(self.collapse_ComboBoxes[i])
@@ -6368,18 +7180,15 @@
 
 
         # Set the collapse visibility based on the field
         self.Populate_collapses()
         
 
     def collapse_type(self, idim):
-
-        '''
-         Set the collapse widget states in plotvars
-        '''
+        '''Set the collapse widget states in plotvars'''
         
         
         f = deepcopy(plotvars.fields[plotvars.index_number])
         mystored = plotvars.stored['f' + str(plotvars.index_number)]
         myaxes = mystored['data_axes']
         myaxes_long = deepcopy(mystored['data_axes'])
         for i in np.arange(len(myaxes_long)):
@@ -6435,17 +7244,15 @@
             
         # Call Populate_collapses for when area is set as both X and Y collapses will change
         self.Populate_collapses()
         
                
         
     def Populate_collapses(self):
-        '''
-         Set the collapse widget visibilities
-        '''        
+        '''Set the collapse widget visibilities'''        
         
         if plotvars.fields is None:
             return
             
             
         f = deepcopy(plotvars.fields[plotvars.index_number])    
             
@@ -6526,15 +7333,15 @@
         # Reset the field title        
         self.parent.reset_field_title()
         
 
                 
 
     def interp_regular(self, text):
-        # Turn sensitvity of interpolation boxes on and off
+        '''Turn sensitvity of interpolation boxes on and off'''
 
         objs = [self.lonminTextBox, self.lonmaxTextBox, self.lonstepTextBox, \
                 self.latminTextBox, self.latmaxTextBox, self.latstepTextBox, \
                 self.lonminLabel, self.lonmaxLabel, self.lonstepLabel, \
                 self.latminLabel, self.latmaxLabel, self.latstepLabel]
 
         if text == 'Off':
@@ -6550,15 +7357,15 @@
             obj.setEnabled(flags[i])
             pal = QPalette(obj.palette())
             pal.setColor(QPalette.WindowText, QColor(color))
             obj.setPalette(pal)
 
 
     def interp_one_to_another(self, text):
-        # Turn sensitvity of interpolation boxes on and off
+        '''Turn sensitvity of interpolation boxes on and off'''
 
         objs = [self.source_ComboBox, self.destination_ComboBox, \
                 self.sourceLabel, self.destinationLabel]
 
         if text == 'Off':
             flags = [False] * 4
         else:
@@ -6573,15 +7380,15 @@
             pal = QPalette(obj.palette())
             pal.setColor(QPalette.WindowText, QColor(color))
             obj.setPalette(pal)
 
 
 
     def checkbox_changed(self, text):
- 
+        '''Change values when a checkbox changes'''
         if text == 'regular':
             if self.interp_regularCheckBox.isChecked():
                 self.interp_to_anotherCheckBox.setChecked(False)
                 self.interp_regular('On')
                 self.interp_one_to_another('Off')
             else:
                 self.interp_regular('Off')
@@ -6594,15 +7401,15 @@
                 self.interp_one_to_another('On')
             else:
                 self.interp_one_to_another('Off')
 
 
 
     def apply(self):
-
+        '''Apply the changes'''
         com_interp = 'import cf\n'
         com_interp += "f = cf.read(" + plotvars.file_read_str + ")"
         if self.interp_regularCheckBox.isChecked():
             com_interp += "[" + str(plotvars.index_number) + "]"
         com_interp += "\n"
         
         changes_made = False
@@ -6637,15 +7444,14 @@
                 changes_made = True
             else:
                 print('Cannot anchor as X does not exist')
                 return
 
 
         if self.reverse_yCheckBox.isChecked():
-
             # Make a copy of the field
             f = deepcopy(plotvars.fields[plotvars.index_number])
 
             if f.has_construct('Y'):
                 f = f.flip('Y')
                 com_interp += "f = f.flip('Y')\n"
                 plotvars.fields[plotvars.index_number] = f
@@ -6759,16 +7565,19 @@
                 com_interp += str(latmax) + ", " + str(latstep) + "), 'degrees_north'))\n"
                 com_interp += "lats.standard_name = 'latitude'\n"
                 com_interp += "lat_bounds = lats.create_bounds(min=-90, max=90)\n"
                 com_interp += "lats.set_bounds(lat_bounds)\n\n"
 
 
                 # Regrid data
-                g = f.regrids({'longitude': lons, 'latitude': lats}, method=method)
-                com_interp += "g = f.regrids({'longitude': lons, 'latitude': lats}, method='" + method + "')\n"
+                # Old code that worked prior to cf-python 3.14.0
+                #g = f.regrids({'longitude': lons, 'latitude': lats}, method=method)
+                #com_interp += "g = f.regrids({'longitude': lons, 'latitude': lats}, method='" + method + "')\n"
+                g = f.regrids([lats, lons], method=method)
+                com_interp += "g = f.regrids([lats, lons], method='" + method + "')\n"                
 
                 changes_made = True
 
             # User supplied grid
             if self.interp_to_anotherCheckBox.isChecked():
 
                 f = deepcopy(plotvars.fields)
@@ -6828,37 +7637,56 @@
         if self.interp_regularCheckBox.isChecked() or self.computationTextBox.text() != '':
             new_name = selected[0].text()
         else:
             source_int = int(self.source_ComboBox.currentText())
             new_name = self.parent.fieldlist.item(source_int).text()
 
         QListWidgetItem(deepcopy(new_name), self.parent.fieldlist)
-        plotvars.stored_dimensions['f' + str(next)] = deepcopy(plotvars.stored_dimensions['f' + str(index)])
-        plotvars.stored_collapses['f' + str(next)] = deepcopy(plotvars.stored_collapses['f' + str(index)])
-        plotvars.stored_collapse_values['f' + str(next)] = deepcopy(plotvars.stored_collapse_values['f' + str(index)])
+        
+
+        
+        orig = deepcopy(plotvars.stored['f' + str(index)])
+        data_axes = orig['data_axes']     
+        axis_sizes = []
+        for j in np.arange(len(data_axes)):
+            axis_sizes.append(len(g.coord(data_axes[j]).array))
+
+        field_dict = {'data_axes': orig['data_axes'],\
+                      'axis_sizes': axis_sizes,\
+                      'axes': [-1] * len(data_axes),\
+                      'collapses': ['Off'] * len(data_axes),\
+                      'collapse_value': False,\
+                      'data_type': orig['data_type'],\
+                      'source': 'Computed',\
+                      'field_name': orig['field_name']}        
+             
+        
+        plotvars.stored['f' + str(next)] = field_dict
+        
+        
         plotvars.fields.append(g)
-        index_length = plotvars.index_length
         new_title = str(next) + (6 - len(str(next))) * ' ' + new_name[6:]
         self.parent.fieldlist.item(next).setText(new_title)
         plotvars.data_source_list.append('interpolated')
         plotvars.index_number = next
         for myselect in selected:
             myselect.setSelected(False)
         self.parent.fieldlist.item(next).setSelected(True)
-         
-        if self.computationTextBox.text() != '':
-            self.parent.fieldlist.item(next).setText(new_title[:30] + 'computed field')
-            
-        plotvars.next_field_index += 1
+        
+        new_title = self.parent.fieldlist.item(next).text()
 
+        plotvars.next_field_index += 1
         changes_made = True
-          
+        
+        plotvars.field_widget_names.append(new_title)
+        
+        
 
     def reset(self):
-        # Reset widget values
+        '''Reset widget values'''
         self.lonminTextBox.setText('')
         self.lonmaxTextBox.setText('')
         self.lonstepTextBox.setText('')
         self.latminTextBox.setText('')
         self.latmaxTextBox.setText('')
         self.latstepTextBox.setText('')
         self.anchorTextBox.setText('')
@@ -6883,15 +7711,15 @@
         self.parent.reset_field_title()
                    
             
 
 
 
     def help(self):
-
+        '''Help for the transform popup'''
         if self.transform_help is None:
 
             html = '<body><h2>Transform help</h2>'
             html += '<h3>Collapse options</h3>'
             html += 'Collapse the field along a dimension with one of the following methods: <br>' 
             html += 'mean, minimumn maximum, variance, standard deviation'
 
@@ -6937,22 +7765,22 @@
             self.transform_help = Help(html)
 
         self.transform_help.show()
 
 
 
     def closeEvent(self, event):
-        # Close self.parent.transform_window
+        '''Close self.parent.transform_window'''
         self.parent.transform_window = None
         self.close()
         
 
 
 class Data_check():
-
+    '''Class for checking data'''
     def __init__(self):
         pass
         
     def test_type(val):  
         # Test if input string is an integer or float
         # Need to match the data to the value
 
@@ -6975,70 +7803,70 @@
             # Float section
             return a
             
         except ValueError:
             return str(val)
 
     def test_numbers(vals):  
-        # Check inputs are numbers
+        '''Check inputs are numbers'''
         vals_okay = True
         errstr = ''
         for val in vals:
             try:
                 float(val)
             except:
                 vals_okay = False
                 errstr += str(val) + ' is not a number\n'
         return vals_okay, errstr
 
     def test_integers(vals):  
-        # Check if all values are integers
+        '''Check if all values are integers'''
         vals_okay = True
         errstr = ''
         for val in vals:
             val_check = val
             if val_check[0] == '-':
                 val_check = val_check[1:]
             if not val_check.isdigit():
                 vals_okay = False
                 errstr += str(val) + ' is not an integer\n'
         return vals_okay, errstr
 
     def test_ascending(vals):  
-        # Check inputs are ascending
+        '''Check inputs are ascending'''
         vals_okay = True
         errstr = ''
         for j in np.arange(np.size(vals) - 1):
             if float(vals[j+1]) <= float(vals[j]):
                 vals_okay = False
                 errstr += 'inputs are not ascending\n'
         return vals_okay, errstr
 
     def test_val0_lt_val1(vals):  
-        # Check min < max
+        '''Check min < max'''
         vals_okay = True
         errstr = ''
         if float(vals[0]) >= float(vals[1]):
             vals_okay = False
             errstr += 'minimum must be less than the maximum\n'
         return vals_okay, errstr
 
     def test_val_gt_zero(val):  
-        # Check step > 0
+        '''Check step > 0'''
         vals_okay = True
         errstr = ''
         if float(val) <= 0:
             vals_okay = False
             errstr += 'step must be greater than zero\n'
         return vals_okay, errstr
 
 
 
 class Cf_funcs():
-
+    '''CF functions class'''
     def __init__(self, parent):
         super(Cf_funcs, self).__init__()
         self.parent = parent
 
         
     def field_name(field=None):
         '''Work out the field name'''
@@ -7151,22 +7979,14 @@
                                 
                     vals.append(myvals)
         
         # Return axis values
         return vals
 
 
-
-
-
-
-
-
-
-
     def field_dims(field=None):
         '''Work out the field dimensions on the original field'''
 
         # Make a copy so any changes are just local
         field = deepcopy(field)
         
         x = []
@@ -7218,33 +8038,28 @@
                 
             if dim == 'T':
                 t = field.construct(dim).dtarray
                 nt = np.size(t)
                 allocated[3] = True
                 plotvars.dim_names[3] = 't'                
                 
-                
-        #print('allocated are', allocated)
-        #print('dim_test are ', dim_test)
         
         
         # Code for dimension coordinates not of form X, Y, Z, T
         if 'dimensioncoordinate' in dim_test:
             
             dims = [x, y, z, t]
             lengths = [nx, ny, nz, nt]
             
             
             # Find unallocated dimension coordinates indicies
             unalloc = [i for i, s in enumerate(dim_test) if 'dimensioncoordinate' in s]
-            #print('unalloc is ', unalloc)
             
             # Find available slots
             avail = [i for i, s in enumerate(allocated) if not s]
-            #print('avail is ', avail)
             
             if len(avail) > 0:
                 for i in np.arange(len(unalloc)):
                     dims[avail[i]] = field.dimension_coordinate(dim_names[avail[i]]).array
                     lengths[avail[i]] = np.size(dims[avail[i]])
                     plotvars.dim_names[avail[i]] = 'dim' + dim_names[avail[i]][-1]
                   
@@ -7425,19 +8240,15 @@
 
             # Work out the widget title
             field_widget_title ='index '
 
             axis_lengths = plotvars.maximum_axis_lengths 
 
             if traj:
-                field_widget_title += 'tracks' + plotvars.maximum_axis_lengths[0] * ' '
-                
-                # ajh - to be deleted
-                #field_widget_title += 'tracks' + (nx_length - 1) * ' '                
-                
+                field_widget_title += 'tracks' + plotvars.maximum_axis_lengths[0] * ' '           
             else:
                 f = plotvars.fields[plotvars.index_number]
                 
                 
 
                 myaxes = plotvars.stored['f' + str(plotvars.index_number)]['data_axes']
                 
@@ -7842,15 +8653,16 @@
         # Strip out any auxiliary coordinates if the field is not a trajectory field
         if remove_aux:
             for i in np.arange(len(dcoords)):
                 if dcoords[i][:-1] == 'auxiliarycoordinate':
                     dcoords[i] = 'aux' 
             dcoords = list(filter(('aux').__ne__,dcoords))
         
-
+        # Test for not removing all auxiliary coordinates
+        remove_aux = False
         
         # Convert these into corresponding dimension coordinates
         if remove_aux:
             coords = []
             for i in np.arange(len(daxes)):
                 val = daxes[i]
                 coord = None
@@ -7874,28 +8686,30 @@
         
         # Convert to X, Y, Z, T if coordinate is one of these
         # If the number of coordinates of this type is greater than 1 then don't do this as f.coord('Z') gives an 
         # error as there are more that one coordinates to return
         #print('daxes are ', daxes)
         #print('coords are ', coords)
         
-        
-        for i in np.arange(len(daxes)):
-            if field.coord(coords[i]).X:
-                if nx == 1:
-                    mycoords[i] = 'X'
-            if field.coord(coords[i]).Y:
-                if ny == 1:
-                    mycoords[i] = 'Y'            
-            if field.coord(coords[i]).Z:
-                if nz == 1:
-                    mycoords[i] = 'Z'  
-            if field.coord(coords[i]).T:
-                if nt == 1:
-                    mycoords[i] = 'T'            
+        # Originally was a loop over daxes
+        #for i in np.arange(len(daxes)):
+        if len(coords) > 0:
+            for i in np.arange(len(coords)):        
+                if field.coord(coords[i]).X:
+                    if nx == 1:
+                        mycoords[i] = 'X'
+                if field.coord(coords[i]).Y:
+                    if ny == 1:
+                        mycoords[i] = 'Y'            
+                if field.coord(coords[i]).Z:
+                    if nz == 1:
+                        mycoords[i] = 'Z'  
+                if field.coord(coords[i]).T:
+                    if nt == 1:
+                        mycoords[i] = 'T'            
             
             
         # Return the reverse of the coordinates so that they are in the order [X, Y, Z, T]
         mycoords.reverse()
         
         daxes = list(field.get_data_axes())
 
@@ -7906,15 +8720,15 @@
         
         
         return mycoords
 
         
                     
     def find_all_dims():
-            
+        '''Find all the dimensions in the field'''
         if plotvars.fields[plotvars.index_number] is not None:
             field = plotvars.fields[plotvars.index_number]
         else:
             return
          
         # Assign lists of data axes and field coordinates   
         daxes = list(field.get_data_axes())
@@ -8043,15 +8857,16 @@
     def __init__(self, parent):
         super(Line_window, self).__init__()
         self.parent = parent
         self.initUI()
 
 
     def initUI(self):
-
+        ''' Main window layout '''
+        
         # Set up the bottom buttons
         resetButton = QPushButton("Reset")
         resetButton.clicked.connect(self.reset)
 
         helpButton = QPushButton("Help")
         helpButton.clicked.connect(self.help)
 
@@ -8261,21 +9076,20 @@
 
         self.data_limits('automatic')
 
         self.show()
 
 
     def line_style(self, text):
-        # Set line type
+        '''Set line type'''
         plotvars.line_style = text
 
 
     def reset(self):
-
-        # Reset line options
+        '''Reset line options'''
 
         self.xminTextBox.setText('')
         self.xmaxTextBox.setText('')
         self.yminTextBox.setText('')
         self.ymaxTextBox.setText('')
         self.titleTextBox.setText('')
         self.markerTextBox.setText('')
@@ -8293,22 +9107,22 @@
         self.line_xmin = None
         self.line_xmax = None
         self.line_ymin = None
         self.line_ymax = None
 
 
     def textbox_changed(self, text):
-
+        '''Change plotvars if a textbox has changed'''
         textbox = getattr(self, text + 'TextBox') 
         setattr(plotvars, 'line_' + text, textbox.text()) 
 
 
 
     def data_limits(self, text):
-
+        '''Change colour and sensitivity and colour of widgets if self.user_data_limitsCheckBox is checked'''
         if self.user_data_limitsCheckBox.isChecked():
             text = 'user'
 
         plotvars.line_limits = text
 
         objs = [self.xminTextBox, self.xmaxTextBox, self.yminTextBox, self.ymaxTextBox,\
                 self.xminLabel, self.xmaxLabel, self.yminLabel, self.ymaxLabel]
@@ -8329,15 +9143,15 @@
             obj.setEnabled(flags[i])
             pal = QPalette(obj.palette())
             pal.setColor(QPalette.WindowText, QColor(color))
             obj.setPalette(pal)
 
 
     def help(self):
-
+        '''Help for the line options popup'''
         if self.line_help is None:
 
             html = '<body><h2>Line plot options</h2>'
             html += '<h3>Line properties</h3>'
             html += 'The default line properties are a solid line of thickness 1.0 and colour C0\n'
             html += 'A list of default line colours is shown at\n'
             html += 'https://matplotlib.org/stable/users/dflt_style_changes.html\n'
@@ -8356,32 +9170,33 @@
             html += 'not the X direction i.e. longitude as specified in the data\n' 
             self.line_help = Help(html)
 
         self.line_help.show()
         
         
     def closeEvent(self, event):
-        # Close self.parent.line_window
+        '''Close self.parent.line_window'''
         self.parent.line_window = None
         self.close()
         
         
 
 
 class Vector_window(QWidget):
-    '''popup window for changing vector defaults'''
+    ''' Popup window for changing vector defaults '''
 
     def __init__(self, parent):
         super(Vector_window, self).__init__()
         self.parent = parent
         self.initUI()
 
 
     def initUI(self):
-
+        ''' Main window layout '''
+        
         # Set up the bottom buttons
         resetButton = QPushButton("Reset")
         resetButton.clicked.connect(self.reset)
 
         helpButton = QPushButton("Help")
         helpButton.clicked.connect(self.help)
 
@@ -8512,26 +9327,27 @@
 
 
         self.show()
 
 
 
     def textbox_changed(self, text):
-    
+        '''Set plotvars variables based on the user text boxes'''
+        
         textbox = getattr(self, 'vector_' + text + 'TextBox') 
         if text == 'title':
             setattr(plotvars, 'vect_' + text, textbox.text()) 
         else:
             val = Data_check.test_type(textbox.text())
             setattr(plotvars, 'vect_' + text, val) 
         
 
     def reset(self):
-
-        # Reset vector options
+        '''Reset vector options'''
+        
         self.vector_titleTextBox.setText('')
         self.vector_scaleTextBox.setText('100')
         self.vector_strideTextBox.setText('')
         self.vector_ptsTextBox.setText('')
         self.vector_key_lengthTextBox.setText('10')
         self.vector_widthTextBox.setText('0.02')
         self.vector_headwidthTextBox.setText('3')        
@@ -8543,15 +9359,16 @@
         plotvars.vect_key_length = 10
         plotvars.vect_pivot = 'middle'
         plotvars.vect_width = 0.02
         plotvars.vect_headwidth = 3
 
 
     def help(self):
-
+        '''Help text for vectors'''
+        
         if self.vector_help is None:
 
             html = '<body><h2>Vector plot options</h2>'
             html += '<h3>Vector properties</h3>'
             html += '<b>title</b> If a title is unset then the title is the u and v fields<br>'
             html += '<b>scale</b> Initially set to 100.  A value of 50 gives vectors that are twice as long<br>'
             html += '<b>pts</b> Interpolate to this number of points in the plot x and y directions<br>'
@@ -8563,33 +9380,35 @@
 
             self.line_help = Help(html)
 
         self.line_help.show()
 
 
     def closeEvent(self, event):
-        # Close parent.vector_window
+        '''Close parent.vector_window'''
+        
         self.parent.vector_window = None
         self.close()
 
 
 
 
 
 class Trajectory_window(QWidget):
-    '''popup window for changing trajectory defaults'''
+    '''Popup window for changing trajectory defaults'''
 
     def __init__(self, parent):
         super(Trajectory_window, self).__init__()
         self.parent = parent
         self.initUI()
 
 
     def initUI(self):
-
+        '''Main window layout'''
+        
         # Set up the bottom buttons
         resetButton = QPushButton("Reset")
         resetButton.clicked.connect(self.reset)
 
         helpButton = QPushButton("Help")
         helpButton.clicked.connect(self.help)
 
@@ -8785,29 +9604,29 @@
         self.window().setFont(custom_font)
 
 
         self.show()
 
 
     def textbox_changed(self, text):
-
+        '''Change plotvars varibles if a textbox changes'''
         textbox = getattr(self, 'trajectory_' + text + 'TextBox') 
         setattr(plotvars, 'trajectory_' + text, textbox.text()) 
 
     def trajectory_line_style(self, text):
-        # Set line type
+        '''Set line type'''
         plotvars.trajectory_line_style = text
 
     def item_clicked(self, item):
+        '''Change plotvars variables when a checkbox is clicked'''
         plotvars.trajectory_vector = self.trajectory_vectorCheckBox.isChecked()
         plotvars.trajectory_legend = self.trajectory_legendCheckBox.isChecked()
 
     def reset(self):
-
-        # Reset vector options
+        '''Reset vector options'''
        
         self.trajectory_titleTextBox.setText('')
         self.trajectory_marker_shapeTextBox.setText('o')
         self.trajectory_marker_sizeTextBox.setText('5')
         self.trajectory_marker_face_colourTextBox.setText('red')
         self.trajectory_marker_edge_colourTextBox.setText('green')
         self.trajectory_line_colourTextBox.setText('blue')
@@ -8827,15 +9646,15 @@
         plotvars.trajectory_line_style ='-'
         plotvars.trajectory_legend = False
         plotvars.trajectory_date_min = ''
         plotvars.trajectory_date_max = ''
 
 
     def help(self):
-
+        '''Help for the trajectory window popup'''
         if self.trajectory_help is None:
 
             html = '<body><h2>Trajectory plot options</h2>'
             html += '<h3>Trajectory properties</h3>'
             html += '<b>title</b> The title of the plot<br>'
             html += '<b>marker shape</b> Marker shape - default is a circle<br>'
             html += '<b>marker size</b> Marker size<br>'
@@ -8851,22 +9670,23 @@
             html += '<br>Line colours  - https://matplotlib.org/stable/gallery/color/named_colors.html<br>'
 
             self.line_help = Help(html)
 
         self.line_help.show()
 
     def closeEvent(self, event):
-        # Close parent.trajectory_window
+        '''Close parent.trajectory_window'''
         self.parent.trajectory_window = None
         self.close()
 
 
 
 
 def main(filename, defaults='~/.cfview_defaults'):
+    '''Main cfview window startup'''
     app = QApplication(sys.argv)
     app.setStyle('Fusion')
 
     ex = Cfview(filename, defaults)
     sys.exit(app.exec_())
 
 if __name__ == '__main__':
```

### Comparing `cf-view-3.1.0/setup.py` & `cf-view-3.2.22/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(name = "cf-view",
     long_description = "GUI for viewing CF files",
-    version      = "3.1.0",
+    version      = "3.2.22",
     description  = "GUI for viewing CF files",
     author       = "Andy Heaps",
     maintainer   = "Andy Heaps",
     maintainer_email  = "andy.heaps@ncas.ac.uk",
     author_email = "andy.heaps@ncas.ac.uk",
     url          = "http://ajheaps.github.io/cf-view",
     download_url = "https://github.com/ajheaps/CF-View",
```

