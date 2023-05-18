# Comparing `tmp/bandplot-0.1.5.1-py3-none-any.whl.zip` & `tmp/bandplot-0.1.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 15058 bytes, number of entries: 11
--rw-rw-r--  2.0 unx       26 b- defN 23-May-16 03:55 bandplot/__init__.py
--rw-rw-r--  2.0 unx     6905 b- defN 23-May-16 03:55 bandplot/mass.py
--rw-rw-r--  2.0 unx    25472 b- defN 23-May-16 03:55 bandplot/plots.py
--rw-rw-r--  2.0 unx    22228 b- defN 23-May-16 03:55 bandplot/pplots.py
--rw-rw-r--  2.0 unx     6349 b- defN 23-May-16 03:55 bandplot/readdata.py
--rw-rw-r--  2.0 unx    22112 b- defN 23-May-16 03:55 bandplot/wrapper.py
--rw-rw-r--  2.0 unx     2996 b- defN 23-May-16 03:55 bandplot-0.1.5.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-16 03:55 bandplot-0.1.5.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       86 b- defN 23-May-16 03:55 bandplot-0.1.5.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-May-16 03:55 bandplot-0.1.5.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      860 b- defN 23-May-16 03:55 bandplot-0.1.5.1.dist-info/RECORD
-11 files, 87135 bytes uncompressed, 13614 bytes compressed:  84.4%
+Zip file size: 17592 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx       26 b- defN 23-May-18 19:19 bandplot/__init__.py
+-rw-rw-r--  2.0 unx     7096 b- defN 23-May-18 19:19 bandplot/mass.py
+-rw-rw-r--  2.0 unx    25644 b- defN 23-May-18 19:19 bandplot/plots.py
+-rw-rw-r--  2.0 unx    22326 b- defN 23-May-18 19:19 bandplot/pplots.py
+-rw-rw-r--  2.0 unx     9321 b- defN 23-May-18 19:19 bandplot/projected.py
+-rw-rw-r--  2.0 unx     6229 b- defN 23-May-18 19:19 bandplot/readdata.py
+-rw-rw-r--  2.0 unx    23352 b- defN 23-May-18 19:19 bandplot/wrapper.py
+-rw-rw-r--  2.0 unx     2996 b- defN 23-May-18 19:20 bandplot-0.1.5.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-18 19:20 bandplot-0.1.5.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       86 b- defN 23-May-18 19:20 bandplot-0.1.5.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-18 19:20 bandplot-0.1.5.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      938 b- defN 23-May-18 19:20 bandplot-0.1.5.2.dist-info/RECORD
+12 files, 98115 bytes uncompressed, 16030 bytes compressed:  83.7%
```

## zipnote {}

```diff
@@ -6,29 +6,32 @@
 
 Filename: bandplot/plots.py
 Comment: 
 
 Filename: bandplot/pplots.py
 Comment: 
 
+Filename: bandplot/projected.py
+Comment: 
+
 Filename: bandplot/readdata.py
 Comment: 
 
 Filename: bandplot/wrapper.py
 Comment: 
 
-Filename: bandplot-0.1.5.1.dist-info/METADATA
+Filename: bandplot-0.1.5.2.dist-info/METADATA
 Comment: 
 
-Filename: bandplot-0.1.5.1.dist-info/WHEEL
+Filename: bandplot-0.1.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: bandplot-0.1.5.1.dist-info/entry_points.txt
+Filename: bandplot-0.1.5.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: bandplot-0.1.5.1.dist-info/top_level.txt
+Filename: bandplot-0.1.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: bandplot-0.1.5.1.dist-info/RECORD
+Filename: bandplot-0.1.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bandplot/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.1.5.1"
+__version__ = "0.1.5.2"
```

## bandplot/mass.py

```diff
@@ -99,18 +99,20 @@
         ticks[0],ticks[-1] = data[0,0],data[-1,0]
         for i in ticks[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
     plt.xticks(ticks,labels)
     plt.xlim(data[0,0],data[-1,0])
     plt.ylim(fig_p.vertical)
     plt.plot(data[:,0], data[:,1:], color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
+    L = plt.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
+    plt.gca().add_artist(L)
     for i in range(len(calM)):
         plt.plot(calM[i][0],calM[i][1], label='%7.3f'%pltlabel[i])
     plt.ylabel('Energy (eV)')
-    plt.legend(frameon=False, loc='upper left', alignment='left', title=legend[0]+'\n$LUMO$ & $HOMO$', title_fontproperties={'size':'medium'})
+    plt.legend(frameon=False, loc='upper left', alignment='left', title='$LUMO$ & $HOMO$', title_fontproperties={'size':'medium'})
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def plot2(data, calM_u, pltlabel_u, calM_d, pltlabel_d, ticks, labels, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(1, 2, figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['darkred', 'red']
     linestyle = fig_p.linestyle or [':', ':']
@@ -122,15 +124,15 @@
     if len(linewidth) == 1:
         linewidth = [linewidth[0], 0.8]
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
-    L = ax1.legend([], frameon=False, loc='lower left', title=legend[0], title_fontproperties={'size':'medium'})
+    L = ax1.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     ax1.add_artist(L)
     if len(ticks) > 2:
         ticks[0],ticks[-1] = data[0,0,0],data[0,-1,0]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
```

## bandplot/plots.py

```diff
@@ -44,15 +44,15 @@
     plt.ylim(fig_p.vertical)
     plt.ylabel('Energy (eV)')
     ax = plt.axes()
     g = ax.plot(arr[1], bands[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
     ax.set_xlim(arr[1][0], arr[1][-1])
     ax.set_ylim(fig_p.vertical)
     ax.axis('off')
-    L = plt.legend([], frameon=False, loc='lower left', title=legend[0], title_fontproperties={'size':'medium'})
+    L = plt.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     plt.gca().add_artist(L)
     plt.legend([f[0], g[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Noneispin3(arr, bands, ticks, labels, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['r', 'k', 'b']
@@ -81,15 +81,15 @@
     ax.set_ylim(fig_p.vertical)
     ax.axis('off')
     af = plt.axes()
     h = ax.plot(arr[2], bands[2].T, color=color[2], linewidth=linewidth[2], linestyle=linestyle[2])
     af.set_xlim(arr[2][0], arr[2][-1])
     af.set_ylim(fig_p.vertical)
     af.axis('off')
-    L = plt.legend([], frameon=False, loc='lower left', title=legend[0], title_fontproperties={'size':'medium'})
+    L = plt.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     plt.gca().add_artist(L)
     plt.legend([f[0], g[0], h[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Ispin(arr, bands, ticks, labels, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['r', 'k']
@@ -128,15 +128,15 @@
         color = [color[0], 'k']
     if len(linestyle) == 1:
         linestyle = [linestyle[0], '-.']
     if len(linewidth) == 1:
         linewidth = [linewidth[0], 0.8]
     ax1.plot(arr, bands[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     ax2.plot(arr, bands[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    L = ax1.legend([], frameon=False, loc='lower left', title=legend[0], title_fontproperties={'size':'medium'})
+    L = ax1.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     ax1.add_artist(L)
     ax1.legend(['up'], frameon=False, prop={'style':'italic', 'size':'medium'}, loc=fig_p.location)
     ax2.legend(['down'], frameon=False, prop={'style':'italic', 'size':'medium'}, loc=fig_p.location)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
 
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
@@ -170,15 +170,15 @@
         color = color + [''] * (4 - len(color))
     if len(linestyle) < 4:
         linestyle = linestyle + ['-'] * (4 - len(linestyle))
     if len(linewidth) < 4:
         linewidth = linewidth + [0.8] * (4 - len(linewidth))
     f1 = ax1.plot(arr[0], bands[0][0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     f2 = ax2.plot(arr[0], bands[0][1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    L = ax1.legend([], frameon=False, loc='lower left', title=legend[0], title_fontproperties={'size':'medium'})
+    L = ax1.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     ax1.add_artist(L)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
 
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
@@ -226,15 +226,15 @@
         color = color + [''] * (6 - len(color))
     if len(linestyle) < 6:
         linestyle = linestyle + ['-'] * (6 - len(linestyle))
     if len(linewidth) < 6:
         linewidth = linewidth + [0.8] * (6 - len(linewidth))
     f1 = ax1.plot(arr[0], bands[0][0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     f2 = ax2.plot(arr[0], bands[0][1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    L = ax1.legend([], frameon=False, loc='lower left', title=legend[0], title_fontproperties={'size':'medium'})
+    L = ax1.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     ax1.add_artist(L)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
 
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
@@ -299,19 +299,19 @@
         linestyle = linestyle + ['-'] * (num + 1 - len(linestyle))
 
     if num + 1 > len(linewidth):
         linewidth = linewidth + [0.8] * (num + 1 - len(linewidth))
 
     for i in range(num):
         if color[i+1]:
-            ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+1], linestyle=linestyle[i+1], color=color[i+1])
+            p_dos += ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+1], linestyle=linestyle[i+1], color=color[i+1])
             if fig_p.fill:
-                plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i+2], alpha=fig_p.fill)
+                plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i+1], alpha=fig_p.fill)
         else:
-            ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+1], linestyle=linestyle[i+1])
+            p_dos += ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+1], linestyle=linestyle[i+1])
             if fig_p.fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=fig_p.fill)
 
     ax1.legend([legend[0]], frameon=False, prop={'size':'small'}, loc=fig_p.location)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.minorticks_on()
     ax2.tick_params(axis='both', which='minor', color='gray')
@@ -358,19 +358,19 @@
         linestyle = linestyle + ['-'] * (num + 2 - len(linestyle))
 
     if num + 2 > len(linewidth):
         linewidth = linewidth + [0.8] * (num + 2 - len(linewidth))
 
     for i in range(num):
         if color[i+2]:
-            p_dos = p_dos + ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2], color=color[i+2])
+            p_dos += ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2], color=color[i+2])
             if fig_p.fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i+2], alpha=fig_p.fill)
         else:
-            p_dos = p_dos + ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2])
+            p_dos += ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2])
             if fig_p.fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=fig_p.fill)
 
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.minorticks_on()
     ax2.tick_params(axis='both', which='minor', color='gray')
     ax2.axvline(linewidth=0.4, linestyle='-.', c='gray')
@@ -402,15 +402,15 @@
         color = [color[0], 'k']
     if len(linestyle) == 1:
         linestyle = [linestyle[0], '-.']
     if len(linewidth) == 1:
         linewidth = [linewidth[0], 0.8]
     ax1.plot(arr, bands[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     ax2.plot(arr, bands[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    L = ax1.legend([], frameon=False, loc='lower left', title=legend[0], title_fontproperties={'size':'small'})
+    L = ax1.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'small'})
     ax1.add_artist(L)
     ax1.legend(['up'], frameon=False, prop={'style':'italic', 'size':'small'}, loc=fig_p.location)
     ax2.legend(['down'], frameon=False, prop={'style':'italic', 'size':'small'}, loc=fig_p.location)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
     ax3.minorticks_on()
     ax3.tick_params(axis='both', which='minor', color='gray')
@@ -423,19 +423,19 @@
         linestyle = linestyle + ['-'] * (num + 2 - len(linestyle))
 
     if num + 2 > len(linewidth):
         linewidth = linewidth + [0.8] * (num + 2 - len(linewidth))
 
     for i in range(num):
         if color[i+2]:
-            p_dos = p_dos + ax3.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2], color=color[i+2])
+            p_dos += ax3.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2], color=color[i+2])
             if fig_p.fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i+2], alpha=fig_p.fill)
         else:
-            p_dos = p_dos + ax3.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2])
+            p_dos += ax3.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2])
             if fig_p.fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=fig_p.fill)
 
     ax3.axvline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
     ax3.set_yticklabels([])
     ax3.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location, alignment='left', title="Density of states", title_fontproperties={'size':'small'})
@@ -481,44 +481,44 @@
 
     if num > len(linewidth):
         linewidth = linewidth + [0.8] * (num - len(linewidth))
 
     if fig_p.exchange:
         for i in range(num):
             if color[i]:
-                p_dos = p_dos + plt.plot(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], linewidth=linewidth[i], linestyle=linestyle[i], color=color[i])
+                p_dos += plt.plot(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], linewidth=linewidth[i], linestyle=linestyle[i], color=color[i])
                 if fig_p.fill:
                     plt.fill_between(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], 0, color=color[i], alpha=fig_p.fill)
             else:
-                p_dos = p_dos + plt.plot(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], linewidth=linewidth[i], linestyle=linestyle[i])
+                p_dos += plt.plot(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], linewidth=linewidth[i], linestyle=linestyle[i])
                 if fig_p.fill:
                     plt.fill_between(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], 0, alpha=fig_p.fill)
 
         plt.tick_params(axis='y', labelsize='medium', labelcolor='dimgray')
         plt.xlim(fig_p.vertical)
         plt.ylim(fig_p.horizontal)
         plt.xlabel('Energy (eV)')
         plt.ylabel('Density of states, electrons/eV')
     else:
         for i in range(num):
             if color[i]:
-                p_dos = p_dos + plt.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=0.8, linestyle=linestyle[i], color=color[i])
+                p_dos += plt.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=0.8, linestyle=linestyle[i], color=color[i])
                 if fig_p.fill:
                     plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i], alpha=fig_p.fill)
             else:
-                p_dos = p_dos + plt.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=0.8, linestyle=linestyle[i])
+                p_dos += plt.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=0.8, linestyle=linestyle[i])
                 if fig_p.fill:
                     plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=fig_p.fill)
 
         plt.tick_params(axis='x', labelsize='medium', labelcolor='dimgray')
         plt.ylim(fig_p.vertical)
         plt.xlim(fig_p.horizontal)
         plt.ylabel('Energy (eV)')
         plt.xlabel('Density of states, electrons/eV')
 
-    L = plt.legend([], frameon=False, loc='lower left', title=legend[0], title_fontproperties={'size':'medium'})
+    L = plt.legend([], frameon=False, loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     plt.gca().add_artist(L)
     plt.axvline(linewidth=0.4, linestyle='-.', c='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
```

## bandplot/pplots.py

```diff
@@ -247,15 +247,16 @@
     L = plt.legend([], frameon=False, loc='upper left', title=legend[0], title_fontproperties={'size':'medium'})
     plt.gca().add_artist(L)
     plt.legend([f[0], g[0], h[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 
 def BrokenWd(arr, fre, ticks, labels, broken, darr, dele, elements, legend, fig_p):
-    fig, ((ax1, ax2), (ax3, ax4)) = plt.subplots(2, 2, height_ratios=[fig_p.height_ratio, 1-fig_p.height_ratio], width_ratios=[1-fig_p.width_ratios, fig_p.width_ratios], figsize=fig_p.size)
+    fig, ((ax1, ax2), (ax3, ax4)) = plt.subplots(2, 2, height_ratios=[fig_p.height_ratio, 1-fig_p.height_ratio],
+                                                 width_ratios=[1-fig_p.width_ratios, fig_p.width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0, hspace=0.0)
     color = fig_p.color or ['r']
     linestyle = fig_p.linestyle or ['-']
     linewidth = fig_p.linewidth or [0.8]
     ax1.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     ax3.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     num = dele.shape[-1]
@@ -317,15 +318,16 @@
     elif num < len(elements):
         if num == 1:
             elements = ['$tdos$']
         else:
             elements = elements[:num]
 
     ax3.legend([legend[0]], frameon=False, prop={'size':'small'}, loc=fig_p.location)
-    ax4.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location, alignment='left', title="Phonon DOS", title_fontproperties={'size':'small'})
+    ax4.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location,
+               alignment='left', title="Phonon DOS", title_fontproperties={'size':'small'})
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax3.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
 
     ax3.set_xticks(ticks,labels)
@@ -385,15 +387,16 @@
         if num == 1:
             elements = ['$tdos$']
         else:
             elements = elements[:num]
 
     ax1.legend([legend[0]], frameon=False, prop={'size':'small'}, loc=fig_p.location)
     ax2.axvline(linewidth=0.4,linestyle='-.',c='dimgray')
-    ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location, alignment='left', title="Phonon DOS", title_fontproperties={'size':'small'})
+    ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location,
+               alignment='left', title="Phonon DOS", title_fontproperties={'size':'small'})
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
 
     ax1.set_xticks(ticks,labels)
     ax1.set_ylabel('Frequency (THz)')
@@ -456,10 +459,11 @@
         elements = elements + [''] * (num - len(elements))
     elif num < len(elements):
         if num == 1:
             elements = ['$tdos$']
         else:
             elements = elements[:num]
 
-    plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, loc=fig_p.location, alignment='left', title=legend[0], title_fontproperties={'size':'medium'})
+    plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, loc=fig_p.location,
+               alignment='left', title=legend[0], title_fontproperties={'size':'medium'})
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
```

## bandplot/readdata.py

```diff
@@ -20,124 +20,123 @@
 def dos(DOS):
     ARR = []
     ELE = []
     s_elements = []
     for pdos in DOS:
         with open(pdos, "r") as main_file:
             first_line = next(main_file)
-        data = np.loadtxt(pdos)
-        arr = data[:, 0]
-        ele = data[:, 1:]
+        dat = np.loadtxt(pdos)
+        arr = dat[:, 0]
+        ele = dat[:, 1:]
         ARR.append(arr)
         ELE.append(ele)
-        s_elements.append([re.sub('.dat|^[A-Za-z]+_', '', pdos)] + first_line.split()[1:])
+        s_elements.append([re.sub('.dat$|^.+PDOS_|^.+/', '', pdos)] + first_line.split()[1:])
     return ARR, ELE, s_elements
 
 def select(s_elements, partial):
     partial = [i for i in partial if i.strip()]
     num = len(s_elements)
     if not partial:
-        index = [(i, -1) for i in range(num)]
+        index = []
+        for i in range(num):
+            if s_elements[i][0] == "TDOS":
+                index += [(i, j) for j in range(1, len(s_elements[i]))]
+            else:
+                index.append((i, -1))
     elif partial[0] == 'all':
         index = [(i, j) for i in range(num) for j in range(1, len(s_elements[i]))]
     else:
         index = []
         for str0 in partial:
             if str0.islower():
                 str_list = str0.split(',')
                 for i, elem in enumerate(s_elements):
-                    for j, sub_elem in enumerate(elem):
-                        if j == 0 or sub_elem not in str_list:
-                            continue
-                        index.append((i, j))
+                    index += [(i, j) for j, sub_elem in enumerate(elem) if j > 0 and sub_elem in str_list]
             else:
                 str_list = [i.strip() for i in str0.split('-') if i.strip()]
                 if len(str_list) == 1:
                     for i, elem in enumerate(s_elements):
-                        if elem[0] == str_list[0] or elem[0] == str_list[0]+'_UP' or elem[0] == str_list[0]+'_DW':
+                        if re.sub('_DW$|_UP$', '', elem[0]) in str_list[0].split(','):
                             index += [(i, j) for j in range(1, len(elem))]
                 elif len(str_list) == 2:
                     for i, elem in enumerate(s_elements):
-                        if elem[0] == str_list[0] or elem[0] == str_list[0]+'_UP' or elem[0] == str_list[0]+'_DW':
-                            index += [(i, j) for j, sub_elem in enumerate(elem)
-                                      if j > 0 and sub_elem in str_list[1].split(',')]
-    labels_elements = [s_elements[i[0]][0].replace('_DW','')+'-$'+s_elements[i[0]][i[1]]+'$'+' ($dw$)' if s_elements[i[0]][0].endswith('_DW')
-                  else s_elements[i[0]][0].replace('_UP','')+'-$'+s_elements[i[0]][i[1]]+'$'+' ($up$)' if s_elements[i[0]][0].endswith('_UP')
-                  else s_elements[i[0]][0]+'-$'+s_elements[i[0]][i[1]]+'$' for i in index]
+                        if re.sub('_DW$|_UP$', '', elem[0]) in str_list[0].split(','):
+                            index += [(i, j) for j, sub_elem in enumerate(elem) if j > 0 and sub_elem in str_list[1].split(',')]
+    labels_elements = [s_elements[i][0].replace('_DW','')+'-$'+s_elements[i][j]+'$'+' ($dw$)' if s_elements[i][0].endswith('_DW')
+                  else s_elements[i][0].replace('_UP','')+'-$'+s_elements[i][j]+'$'+' ($up$)' if s_elements[i][0].endswith('_UP')
+                  else s_elements[i][0]+'-$'+s_elements[i][j]+'$' for i, j in index]
     index_f = [(i, j-1) if j > 0 else (i, j) for i, j in index]
     return index_f, labels_elements
 
 def bands(PLOT):
     with open(PLOT, "r") as main_file:
         lines = main_file.readlines()
     str0 = lines[0].split()
-    if len(str0) == 2 and str0[1] == "Energy-Level(eV)":
+    if len(str0) == 3 and str0[1] == "Spin-Up(eV)" and str0[2] == "Spin-down(eV)":
         nkps = re.sub(':', ' ', lines[1]).split()
         m, n = int(nkps[-2]), int(nkps[-1])
         arr = np.zeros(m)
-        bands = np.zeros((n,m))
+        ban = np.zeros((2,n,m))
         reverse = False
         for i in lines[2:]:
             str = i.split()
             if i[0] == '#':
                 j = int(str[-1])
                 k = 0
             elif len(str) > 0:
                 if j == 1:
-                    arr[k], bands[0,k] = float(str[0]), float(str[1])
+                    arr[k], ban[0,0,k], ban[1,0,k] = float(str[0]), float(str[1]), float(str[2])
                     k += 1
                 else:
                     N = j - 1
                     if k == 0:
                         if float(str[0]) == 0:
                             reverse = False
                         else:
                             reverse = True
                     if reverse:
                         K = m-k-1
                     else:
                         K = k
-                    bands[N,K] = float(str[1])
+                    ban[0,N,K], ban[1,N,K] = float(str[1]), float(str[2])
                     k += 1
             else:
                 pass
-        return arr, bands, "Noneispin"
-    elif len(str0) == 3 and str0[1] == "Spin-Up(eV)" and str0[2] == "Spin-down(eV)":
-        nkps = lines[1].split()
+        return arr, ban, "Ispin"
+    else:
+        nkps = re.sub(':', ' ', lines[1]).split()
         m, n = int(nkps[-2]), int(nkps[-1])
         arr = np.zeros(m)
-        bands = np.zeros((2,n,m))
+        ban = np.zeros((n,m))
         reverse = False
         for i in lines[2:]:
             str = i.split()
             if i[0] == '#':
                 j = int(str[-1])
                 k = 0
             elif len(str) > 0:
                 if j == 1:
-                    arr[k], bands[0,0,k], bands[1,0,k] = float(str[0]), float(str[1]), float(str[2])
+                    arr[k], ban[0,k] = float(str[0]), float(str[1])
                     k += 1
                 else:
                     N = j - 1
                     if k == 0:
                         if float(str[0]) == 0:
                             reverse = False
                         else:
                             reverse = True
                     if reverse:
                         K = m-k-1
                     else:
                         K = k
-                    bands[0,N,K], bands[1,N,K] = float(str[1]), float(str[2])
+                    ban[N,K] = float(str[1])
                     k += 1
             else:
                 pass
-        return arr, bands, "Ispin"
-    else:
-        pass
+        return arr, ban, "Noneispin"
 
 def symbols(POSCAR):
     with open(POSCAR, "r") as main_file:
         lines = main_file.readlines()
     symbol = lines[5].split()
     factor = [int(i) for i in lines[6].split()]
     return symbol, factor
```

## bandplot/wrapper.py

```diff
@@ -35,14 +35,15 @@
     parser.add_argument('-c', "--color",      type=str,             nargs='+', help="line color: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow;"+
                                                                                     "k, black; w, white", default=[])
     parser.add_argument('-k', "--linestyle",  type=str,             nargs='+', help="linestyle: solid, dashed, dashdot, dotted or tuple; default: solid",
                                                                                     default=[])
     parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', help="linewidth, default: 0.8", default=[])
     parser.add_argument('-m', "--mass",       action='store_true',  help='calculate the effective masses')
     parser.add_argument('-M', "--scale",      type=float,           help='the scale of data for effective masses calculation, default: 0.15', default=0.15)
+    parser.add_argument('-r', "--projected",  action='store_true',  help='plot the projected band structure')
     parser.add_argument('-i', "--input",      type=str,             nargs='+', help="plot figure from .dat file, default: BAND.dat", default=["BAND.dat"])
     parser.add_argument('-o', "--output",     type=str,             help="plot figure filename, default: BAND.png", default="BAND.png")
     parser.add_argument('-q', "--dpi",        type=int,             help="dpi of the figure, default: 500", default=500)
     parser.add_argument('-j', "--klabels",    type=str,             help="filename of KLABELS, default: KLABELS", default="KLABELS")
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
     parser.add_argument('-d', "--dos",        type=str,             nargs='+', default=[], help="plot DOS from .dat file, or file list")
     parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Density of states, electrons/eV range")
@@ -160,14 +161,34 @@
                     else:
                         print("{:<8s}".format('-'), end='')
                 print()
             else:
                 print("ERROR: Input file mismatch.")
         else:
             print("ERROR: BAND_GAP file does not exist.")
+# plot Projected Band Structure
+    elif args.projected:
+        if not fig_p.vertical:
+            fig_p.vertical = [-5.0, 5.0]
+        bandfile = [f for i in ['PBAND_*.dat'] for f in glob.glob(i)] if len(args.input) == 1 and args.input[0] == 'BAND.dat' \
+                    else [f for i in args.input for f in glob.glob(i)]
+        if bandfile:
+            from bandplot import projected
+            darr, dbands, composition, s_elements = projected.bands(bandfile)
+            index_f, labels_elements = projected.select(s_elements, args.partial)
+            if len(index_f) > 0:
+                ispin = [0 if s_elements[i][0].endswith('_DW') else 1 for i, j in index_f]
+                if not elements:
+                    elements = labels_elements
+                if all(x == ispin[0] for x in ispin):
+                    projected.pplot(darr, dbands, composition, ticks, labels, index_f, elements, legend, fig_p)
+                else:
+                    projected.pplot2(darr, dbands, composition, ticks, labels, index_f, elements, ispin, legend, fig_p)
+            else:
+                print("ERROR: Input mismatch.")
 # plot Band Structure
     else:
         bandfile = [f for i in args.input for f in glob.glob(i)]
         len_bandfile = len(bandfile)
         if len_bandfile == 1:
             if not fig_p.vertical:
                 fig_p.vertical = [-5.0, 5.0]
@@ -204,15 +225,15 @@
                     elements = labels_elements
                 if fig_p.fill:
                     fig_p.fill = args.alpha
 
                 plots.pdosfiles(darr, dele, index_f, elements, legend, fig_p)
             else:
                 print("ERROR: No *.dat file.")
-# compare two Band structures
+# compare two Band Structures
         elif len_bandfile == 2:
             if not fig_p.vertical:
                 fig_p.vertical = [-5.0, 5.0]
             arr =   [''] * 2
             bands = [''] * 2
             ispin = [''] * 2
             arr[0], bands[0], ispin[0] = readdata.bands(bandfile[0])
@@ -220,15 +241,15 @@
             if len(legend) < 3:
                 legend = legend + [''] * (3 - len(legend))
 
             if all(x == "Noneispin" for x in ispin):
                 plots.Noneispin2(arr, bands, ticks, labels, legend, fig_p)
             elif all(x == "Ispin" for x in ispin):
                 plots.Dispin2(arr, bands, ticks, labels, legend, fig_p)
-# compare three Band structures
+# compare three Band Structures
         elif len_bandfile == 3:
             if not fig_p.vertical:
                 fig_p.vertical = [-5.0, 5.0]
             arr =   [''] * 3
             bands = [''] * 3
             ispin = [''] * 3
             arr[0], bands[0], ispin[0] = readdata.bands(bandfile[0])
@@ -373,15 +394,15 @@
                     fig_p.output = "DOS.png"
             darr, dele = readdata.pdos(args.dos)
             if fig_p.fill:
                 fig_p.fill = args.alpha
             pplots.dosfile(darr, dele, elements, legend, fig_p)
         else:
             print('No *.dat file.')
-# compare two Phonon Band structures
+# compare two Phonon Band Structures
     elif len_bandfile == 2:
         arr = [''] * 2
         fre = [''] * 2
         ticks = [''] * 2
         arr[0], fre[0], ticks[0] = readdata.pbands(bandfile[0])
         arr[1], fre[1], ticks[1] = readdata.pbands(bandfile[1])
         if len(ticks[0]) > len(labels):
@@ -391,15 +412,15 @@
         if len(legend) < 3:
             legend = legend + [''] * (3 - len(legend))
 
         if args.broken is None:
             pplots.Nobroken2(arr, fre, ticks[0], labels, legend, fig_p)
         else:
             pplots.Broken2(arr, fre, ticks[0], labels, broken, legend, fig_p)
-# compare three Phonon Band structures
+# compare three Phonon Band Structures
     elif len_bandfile == 3:
         arr = [''] * 3
         fre = [''] * 3
         ticks = [''] * 3
         arr[0], fre[0], ticks[0] = readdata.pbands(bandfile[0])
         arr[1], fre[1], ticks[1] = readdata.pbands(bandfile[1])
         arr[2], fre[2], ticks[2] = readdata.pbands(bandfile[2])
```

## Comparing `bandplot-0.1.5.1.dist-info/METADATA` & `bandplot-0.1.5.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandplot
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: Band structure, DOS or phonon band structure plot from vaspkit or phonopy result.
 Home-page: https://github.com/lkccrr/bandplot
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
 Keywords: DFT VASP DOS band plot Phonon
 Platform: Unix
```

