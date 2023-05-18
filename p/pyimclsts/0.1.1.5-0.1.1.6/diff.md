# Comparing `tmp/pyimclsts-0.1.1.5.tar.gz` & `tmp/pyimclsts-0.1.1.6.tar.gz`

## Comparing `pyimclsts-0.1.1.5.tar` & `pyimclsts-0.1.1.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.5/example/followRef.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.5/example/lsf2csv.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.5/example/selectedlsf2csv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.5/src/pyimclsts/__init__.py
--rw-r--r--   0        0        0    17450 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.5/src/pyimclsts/_base_templates.py
--rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.5/src/pyimclsts/core.py
--rw-r--r--   0        0        0    16423 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.5/src/pyimclsts/extract.py
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.5/src/pyimclsts/extractutils.py
--rw-r--r--   0        0        0    32202 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.5/src/pyimclsts/network.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.5/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.5/LICENSE
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.5/README.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.5/pyproject.toml
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.6/example/followRef.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.6/example/lsf2csv.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.6/example/selectedlsf2csv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.6/src/pyimclsts/__init__.py
+-rw-r--r--   0        0        0    17450 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.6/src/pyimclsts/_base_templates.py
+-rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.6/src/pyimclsts/core.py
+-rw-r--r--   0        0        0    16457 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.6/src/pyimclsts/extract.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.6/src/pyimclsts/extractutils.py
+-rw-r--r--   0        0        0    32188 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.6/src/pyimclsts/network.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.6/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.6/LICENSE
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.6/README.md
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.6/PKG-INFO
```

### Comparing `pyimclsts-0.1.1.5/example/followRef.py` & `pyimclsts-0.1.1.6/example/followRef.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.5/example/lsf2csv.py` & `pyimclsts-0.1.1.6/example/lsf2csv.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.5/example/selectedlsf2csv.py` & `pyimclsts-0.1.1.6/example/selectedlsf2csv.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,49 +31,44 @@
         '''f is file name'''
 
         self.file_name = f
         # erases the file if it exists, creates it otherwise
         with open(f, 'w'):
             pass
 
-        self.unwanted_messages = [262, 276, 294]
-        self.selected_messages = list(filter(lambda x : x not in self.unwanted_messages, range(250, 300)))
-
         self.datatable = []
         self.estimated_states = []
             
     def writetotable(self, msg, callback) -> str:
         
-        if msg._header.mgid in self.selected_messages:
-            time = msg._header.timestamp
-            message_abbrev = msg.Attributes.abbrev
-            src = msg._header.src
-            src_ent = msg._header.src_ent
-            
-            data = tolist(msg)
-            data = [[time, message_abbrev, src, src_ent, *d] for d in data] # i don't think it expects a list with more than 1 item.
-            self.datatable += data
+        time = msg._header.timestamp
+        message_abbrev = msg.Attributes.abbrev
+        src = msg._header.src
+        src_ent = msg._header.src_ent
+        
+        data = tolist(msg)
+        data = [[time, message_abbrev, src, src_ent, *d] for d in data] # i don't think it expects a list with more than 1 item.
+        self.datatable += data
 
-        elif isinstance(msg, pg.messages.EstimatedState):
-            time = msg._header.timestamp
+    def update_state(self, msg, callback):
+        time = msg._header.timestamp
             
-            point = [msg.lat, msg.lon, msg.depth, time]
-            
-            self.estimated_states.append(point)
-        else:
-            pass
-
-w = table('output.csv')
+        point = [msg.lat, msg.lon, msg.depth, time]
+        
+        self.estimated_states.append(point)
 
 if __name__ == '__main__':
     
+    w = table('output.csv')
+
     src_file = 'Data.lsf'
     sub = n.subscriber(n.file_interface(input = src_file), use_mp=True)
 
-    sub.subscribe_async(w.writetotable)
+    sub.subscribe_async(w.writetotable, msg_id =pg.messages.Temperature, src='lauv-noptilus-1', src_ent='AHRS')
+    sub.subscribe_async(w.update_state, msg_id =pg.messages.EstimatedState, src='lauv-noptilus-1', src_ent=None)
 
     sub.run()
 
     positions = pd.DataFrame(w.estimated_states, columns=['lat', 'lon', 'depth', 'timestamp'])
     values = pd.DataFrame(w.datatable, columns=['timestamp', 'message', 'src', 'src_ent','field', 'value'])
 
     interpolator = lambda x, key : np.interp(x, positions['timestamp'], positions[key])
@@ -81,12 +76,8 @@
     keys = ['lat', 'lon', 'depth']
     for k in keys:
         values[k] = interpolator(values['timestamp'], k)
 
     metadata = pd.read_csv('AUV_General_Metadata.csv', delimiter=';')
     metadata = metadata.groupby(by = 'Variable Name')
 
-    netcdf_DS = xra.Dataset.from_dataframe(values)
-    
-    #netcdf_DS.timestamp.attrs['oi'] = 'oi'
-    
-    #xra.open_dataset(netcdf_DS.to_netcdf())
+    netcdf_DS = xra.Dataset.from_dataframe(values)
```

### Comparing `pyimclsts-0.1.1.5/src/pyimclsts/_base_templates.py` & `pyimclsts-0.1.1.6/src/pyimclsts/_base_templates.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.5/src/pyimclsts/core.py` & `pyimclsts-0.1.1.6/src/pyimclsts/core.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.5/src/pyimclsts/extract.py` & `pyimclsts-0.1.1.6/src/pyimclsts/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         \'\'\'Class constructor
         
         A (received) message whose format is not known. It has valid sync number and valid CRC but could not be parsed.
 
         This message class contains the following fields and their respective types:
         contents : rawdata, unit: NOT FOUND
         \'\'\'
-        self._Attributes = _base_templates.MessageAttributes(fields = ('contents','endianess', ), name = "Unknown", flags = None, id = id, abbrev = "Unknown", description = "A (received) message whose format is not known. It has valid sync number and valid CRC but could not be parsed.", stable = None, source = None, usedby = None, category = None)
+        self._Attributes = _base_templates.MessageAttributes(fields = ('contents','endianess', ), name = "Unknown", id = id, abbrev = "Unknown", description = "A (received) message whose format is not known. It has valid sync number and valid CRC but could not be parsed.", ##ATTRIBUTES##)
         self._contents = contents
         self._endianess = endianess
     
     def _pack_fields(self, *, serial_functions : dict) -> bytes:
         raise NotImplemented
 
     def pack(self, *, is_field_message : bool = False, is_big_endian : bool = True, src : int = None, src_ent : int = None, 
@@ -71,18 +71,18 @@
 help_text = '''This script generates files that contain python classes as described in the IMC message schema.
 
 Regardless of the chosen option, minimal will always be generated.
 
 Provide a file as parameter, that contains a list of messages (abbrev's, one per line) to be white- or blacklisted.
 '''
 
-minimal = {'EntityState', 'QueryEntityState', 'EntityInfo', 'QueryEntityInfo', 'EntityList', 'EntityActivationState', 'QueryEntityActivationState', 
-           'Heartbeat', 'Announce', 'AnnounceService', 'PlanControl', 'PlanSpecification', 'PlanVariable', 'PlanManeuver', 'PlanTransition'}
+minimal = {'Abort', 'EntityState', 'QueryEntityState', 'EntityInfo', 'QueryEntityInfo', 'EntityList', 'EntityActivationState', 'QueryEntityActivationState', 
+           'Heartbeat', 'Announce', 'AnnounceService'}
 
-def hardcode_message_extractor(message : dict, templates_namespace : str) -> str:
+def hardcode_message_extractor(message : dict, templates_namespace : str, message_attributes : set) -> str:
     description = message.get('description', '')
     name = message['abbrev']
     
     namespace =  templates_namespace + '.' if templates_namespace else ''
 
     ws = '    '
 
@@ -98,15 +98,15 @@
         if attribute in message:
             if attribute == 'fields':
                 value = '({},)'.format(', '.join(["'{}'".format(x) for x in message[attribute].keys()]))
             else:
                 value = str(message[attribute]) if isinstance(message[attribute], int) else '\"' + message[attribute].replace('"','\\"') + '\"'
         else:
             value = '[]' if attribute == 'fields' else 'None'
-        attributes.append(attribute.replace('-','') + ' = ' + value)
+        attributes.append(attribute + ' = ' + value)
     
     for field in message.get('fields', []):
         priv_attrib.append('_' + field)
         initialization_values.append(2*ws + 'self.' + priv_attrib[-1] + ' = ' + field + '\n')
         constructor_args.append(field + ' = None')
         
         # All fields' contents are mutable
@@ -286,19 +286,19 @@
                         int if 'integer' in metadata_encyclopedia['types']['types'][t]['description'] else \
                         None
     imc_types['rawdata'] = bytes
     imc_types['plaintext'] = str
     imc_types['message'] = '<class \'IMC_message\'>'
     imc_types['message-list'] = list
 
-    # XML variables inspection: Check all possible attributes. For dev purpose 
+    # XML variables inspection: Get all possible attributes.
     message_attributes = set()
     for message in message_encyclopedia:
         for attrib in message_encyclopedia[message]:
-            message_attributes.add(attrib)
+            message_attributes.add(attrib.replace('-',''))
 
     fields_attributes = set()
     for message in message_encyclopedia:
         for attrib in message_encyclopedia[message].get('fields', []):
             for child_attrib in message_encyclopedia[message]['fields'][attrib]:
                 fields_attributes.add(child_attrib)
 
@@ -343,20 +343,20 @@
 
     file_name = 'messages.py'
     with open(_target_folder + '/' + file_name, mode = 'w', encoding='utf-8') as f:
         f.write('\'\'\'\nIMC messages.\n\'\'\'\n\n')
         # write import statements
         f.write('from . import _base_templates\nimport enum as _enum\nimport pyimclsts.core as core\n')
         f.write('\n_message_ids = {}\n'.format(str(dict((k, v['abbrev']) for k, v in message_encyclopedia.items()))))
-        f.write(unknown_message)
+        f.write(unknown_message.replace('##ATTRIBUTES##', ', '.join([i + '= None' for i in message_attributes if i not in {'fields', 'name', 'id', 'abbrev', 'description'}])))
         for k, v in message_encyclopedia.items():
-            f.write(hardcode_message_extractor(v, '_base_templates'))
+            f.write(hardcode_message_extractor(v, '_base_templates', message_attributes))
             pass
 
     generated_files = os.listdir(_target_folder)
 
     file_name = '__init__.py'
     with open(_target_folder + '/' + file_name, mode = 'w', encoding='utf-8') as f:
         for name in generated_files:
             f.write('from . import {}\n'.format(name[:-3]))
 
-    print('Finished extracting messages.')
+    print('Finished extracting messages.')
```

### Comparing `pyimclsts-0.1.1.5/src/pyimclsts/extractutils.py` & `pyimclsts-0.1.1.6/src/pyimclsts/extractutils.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.5/src/pyimclsts/network.py` & `pyimclsts-0.1.1.6/src/pyimclsts/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,111 +22,119 @@
 
 _spec = _import.spec_from_file_location(_module_name, _location)
 
 _pg = _import.module_from_spec(_spec)
 _sys.modules[_module_name] = _pg
 _spec.loader.exec_module(_pg)
 
-def unpack(message : bytes, *, is_big_endian : bool, is_field_message : bool = False, fast_mode : bool = False) -> _pg._base_templates.IMC_message:
-    '''Expects a serializable (= exactly long (header + fields + CRC)) string of bits, but may fail (returns None)
-    if the string is invalid. 
+def unpack(message : bytes, *, is_big_endian : bool = None, is_field_message : bool = False, fast_mode : bool = False) -> _pg._base_templates.IMC_message:
+    '''Expects a serializable (= exactly long (header + fields + CRC)) string of bits whose CRC has already been checked
     
     Fast mode skips all type checking performed by the descriptor by directly invoking the constructor.
     '''
+    if is_big_endian is None:
+        is_big_endian = int.from_bytes(message[:2], byteorder='big') == _pg._base_templates._sync_number
+        # Note: is_big_endian is a function parameter to enable recursion
+    
     unpack_functions = _core.unpack_functions_big if is_big_endian else _core.unpack_functions_little
     cursor = 0
     
     if not is_field_message:
         # deserialize header
         (m, size) = unpack_functions['header'](message[cursor:])
         deserialized_header = _pg._base_templates.header_data(*m)
         cursor += size
-        # Magic number 2 = CRC size in bytes
-        contents = message[:-2]
-        crc = unpack_functions['uint16_t'](message[-2:])[0]
-        crc_valid = crc == _core.CRC16IMB(contents)
-    else:
-        crc_valid = None
     
-    # check CRC-16.
-    if crc_valid or is_field_message:
-        if is_field_message:
-            msgid = unpack_functions['uint16_t'](message[cursor:cursor+2])[0]
-            cursor += 2
-        else:
-            msgid = deserialized_header.mgid
-            if msgid not in _pg.messages._message_ids:
-                unknown_msg = _pg.messages.Unknown(msgid, contents = message[cursor:-2], endianess = is_big_endian)
-                unknown_msg._header = deserialized_header
-                return unknown_msg
-        
-        if fast_mode:
-            # get corresponding class
-            message_class = getattr(_pg.messages, _pg.messages._message_ids.get(msgid, None))
-
-            fields = [(f, getattr(getattr(type(message_class()), f), '_field_def')['type']) for f in message_class()._Attributes.fields]
-            arguments = dict()
-            for field, t in fields:
-                if t == 'message':
-                    if unpack_functions['uint16_t'](message[cursor:cursor+2])[0] == 65535:
-                        cursor += 2
-                    else:
-                        (m, size) = unpack(message[cursor:], is_big_endian=is_big_endian, is_field_message=True, fast_mode=fast_mode)
-                        arguments[field] = m
-                        cursor += size
-                elif t == 'message-list':
-                    (n, _) = unpack_functions['uint16_t'](message[cursor:])
+        msgid = deserialized_header.mgid
+        if msgid not in _pg.messages._message_ids:
+            unknown_msg = _pg.messages.Unknown(msgid, contents = message[cursor:-2], endianess = is_big_endian)
+            unknown_msg._header = deserialized_header
+            return unknown_msg
+    else:
+        msgid = unpack_functions['uint16_t'](message[cursor:cursor+2])[0]
+        cursor += 2
+        if msgid not in _pg.messages._message_ids:
+            raise KeyError(f'Cannot parse/unpack an unknown inlined message (no information about the size). Add message id {msgid} to extract list')
+    
+    if fast_mode:
+        # get corresponding class
+        message_class = getattr(_pg.messages, _pg.messages._message_ids.get(msgid, None))
+
+        fields = [(f, getattr(getattr(type(message_class()), f), '_field_def')['type']) for f in message_class()._Attributes.fields]
+        arguments = dict()
+        for field, t in fields:
+            if t == 'message':
+                if unpack_functions['uint16_t'](message[cursor:cursor+2])[0] == 65535:
                     cursor += 2
-                    arguments[field] = []
-                    for _ in range(n):
-                        (m, size) = unpack(message[cursor:], is_big_endian=is_big_endian, is_field_message=True, fast_mode=fast_mode)
-                        arguments[field].append(m)
-                        cursor += size
                 else:
-                    (m, size) = unpack_functions[t](message[cursor:])
+                    (m, size) = unpack(message[cursor:], is_big_endian=is_big_endian, is_field_message=True, fast_mode=fast_mode)
                     arguments[field] = m
                     cursor += size
-            # instantiate class through constructor
-            message_class = message_class(**arguments)
-            
-        else:
-            # instantiate empty class
-            message_class = getattr(_pg.messages, _pg.messages._message_ids.get(msgid, None))()
+            elif t == 'message-list':
+                (n, _) = unpack_functions['uint16_t'](message[cursor:])
+                cursor += 2
+                arguments[field] = []
+                for _ in range(n):
+                    (m, size) = unpack(message[cursor:], is_big_endian=is_big_endian, is_field_message=True, fast_mode=fast_mode)
+                    arguments[field].append(m)
+                    cursor += size
+            else:
+                (m, size) = unpack_functions[t](message[cursor:])
+                arguments[field] = m
+                cursor += size
+        # instantiate class through constructor
+        message_class = message_class(**arguments)
+        
+    else:
+        # instantiate empty class
+        message_class = getattr(_pg.messages, _pg.messages._message_ids.get(msgid, None))()
 
-            # deserialize fields
-            # make a (field, type) tuple list, get information in the descriptor
-            fields = [(f, getattr(getattr(type(message_class), f), '_field_def')['type']) for f in message_class._Attributes.fields]
-            for field, t in fields:
-                if t == 'message':
-                    if unpack_functions['uint16_t'](message[cursor:cursor+2])[0] == 65535:
-                        cursor += 2
-                    else:
-                        (m, size) = unpack(message[cursor:], is_big_endian=is_big_endian, is_field_message=True, fast_mode=fast_mode)
-                        cursor += size
-                        setattr(message_class, field, m)
-                elif t == 'message-list':
-                    (n, _) = unpack_functions['uint16_t'](message[cursor:])
+        # deserialize fields
+        # make a (field, type) tuple list, get information in the descriptor
+        fields = [(f, getattr(getattr(type(message_class), f), '_field_def')['type']) for f in message_class._Attributes.fields]
+        for field, t in fields:
+            if t == 'message':
+                if unpack_functions['uint16_t'](message[cursor:cursor+2])[0] == 65535:
                     cursor += 2
-                    message_list = []
-                    for _ in range(n):
-                        (m, size) = unpack(message[cursor:], is_big_endian=is_big_endian, is_field_message=True, fast_mode=fast_mode)
-                        message_list.append(m)
-                        cursor += size
-                    setattr(message_class, field, message_list)
                 else:
-                    (m, size) = unpack_functions[t](message[cursor:])
+                    (m, size) = unpack(message[cursor:], is_big_endian=is_big_endian, is_field_message=True, fast_mode=fast_mode)
                     cursor += size
                     setattr(message_class, field, m)
+            elif t == 'message-list':
+                (n, _) = unpack_functions['uint16_t'](message[cursor:])
+                cursor += 2
+                message_list = []
+                for _ in range(n):
+                    (m, size) = unpack(message[cursor:], is_big_endian=is_big_endian, is_field_message=True, fast_mode=fast_mode)
+                    message_list.append(m)
+                    cursor += size
+                setattr(message_class, field, message_list)
+            else:
+                (m, size) = unpack_functions[t](message[cursor:])
+                cursor += size
+                setattr(message_class, field, m)
+    
+    if not is_field_message:
+        message_class._header = deserialized_header
+        return message_class
+    else:
+        return (message_class, cursor)
+
+def _get_id_src_src_ent(message : bytes) -> int:
+    src_ent = message[16]
+    if int.from_bytes(message[:2], byteorder='big') == _pg._base_templates._sync_number:
+        id = int.from_bytes(message[2:4], byteorder='big')
+        src = int.from_bytes(message[14:16], byteorder='big')
         
-        if not is_field_message:
-            message_class._header = deserialized_header
-            return message_class
-        else:
-            return (message_class, cursor)
-    return None
+        return (id, src, src_ent)
+    else:
+        id = int.from_bytes(message[2:4], byteorder='little')
+        src = int.from_bytes(message[14:16], byteorder='little')
+        
+        return (id, src, src_ent)
 
 # Re-export some classes:
 
 tcp_interface = _core.tcp_interface
 file_interface = _core.file_interface
 
 class _message_bus():
@@ -310,18 +318,14 @@
         The _external_listener_loop is supposed to send complete messages (as per multiprocessing 
         documentation).'''       
         msg = self._parent_end.recv_bytes()
         
         if msg == b'':
             raise EOFError('Message Bus has been closed.')
         else:
-            if int.from_bytes(msg[:2], byteorder='big') == 0xFE54:
-                msg = unpack(msg, is_big_endian=True, fast_mode=True)
-            else:
-                msg = unpack(msg, is_big_endian=False, fast_mode=True)
             return msg
             
     def poll(self, timeout : int = 0) -> bool:
         '''Extra function to check whether there are any available messages.
         Check _multiprocessing module pipes.
         '''
         return self._parent_end.poll(timeout=timeout)
@@ -457,18 +461,14 @@
         documentation).'''
 
         msg = await self._reader_queue.get()
         
         if msg == b'':
             raise EOFError('No more bytes to read.')
         else:
-            if int.from_bytes(msg[:2], byteorder='big') == 0xFE54:
-                msg = unpack(msg, is_big_endian=True, fast_mode=True)
-            else:
-                msg = unpack(msg, is_big_endian=False, fast_mode=True)
             return msg
             
     def poll(self, timeout : int = 0) -> bool:
         '''Extra function to check whether there are any available messages.
         '''
         return not self._reader_queue.empty()
     
@@ -545,20 +545,22 @@
                 elif callable(f):
                     tasks.append(loop.create_task(self._periodic_wrapper(period, f, msg_mgr.send)))
                 else:
                     print(f'Warning: Given function {f} is neither _typing.Callable nor a coroutine.')
 
             while True:
                 msg = msg_mgr.recv() if self._use_mp else await msg_mgr.recv()
-                if msg._header.mgid in self._subscriptions:
-                    for f in self._subscriptions[msg._header.mgid]:
-                        if self._validate_call(msg, f[1], f[2]):
-                            await f[0](msg, msg_mgr.send)
+                mgid, src, src_ent = _get_id_src_src_ent(msg)
+                if mgid in self._subscriptions:
+                    desel_message = unpack(msg, fast_mode=True)
+                    for f in self._subscriptions[mgid]:
+                        if self._validate_call(src, src_ent, f[1], f[2]):
+                            await f[0](desel_message, msg_mgr.send)
                 
-                [await f[0](msg, msg_mgr.send) for f in self._subscripted_all if self._validate_call(msg, f[1], f[2])]
+                [await f[0](unpack(msg, fast_mode=True), msg_mgr.send) for f in self._subscripted_all if self._validate_call(src, src_ent, f[1], f[2])]
                 # Offer an exit point
                 await _asyncio.sleep(0)
         except EOFError:
             print('Stream has ended.')
         finally:
             msg_mgr.close()
 
@@ -607,20 +609,20 @@
             return entityList.get(entityName, None)
         return None
     
     def _queryEntityList(self, send):
         query = _pg.messages.EntityList(op=_pg.messages.EntityList.OP.QUERY, list='')
         send(query)
     
-    def _validate_call(self, msg, desired_src : str, desired_src_ent : str) -> bool:
+    def _validate_call(self, src, src_ent, desired_src : str, desired_src_ent : str) -> bool:
         if desired_src is None and desired_src_ent is None:
             return True
         else:
-            correct_src = msg._header.src == self._get_src(desired_src) 
-            correct_src_ent = msg._header.src_ent == self._get_src_ent(desired_src, desired_src_ent)
+            correct_src = src == self._get_src(desired_src) 
+            correct_src_ent = src_ent == self._get_src_ent(desired_src, desired_src_ent)
             
             if (correct_src or correct_src_ent) and (desired_src is None or desired_src_ent is None):
                 return True
             elif correct_src and correct_src_ent:
                 return True
             
         return False
```

### Comparing `pyimclsts-0.1.1.5/.gitignore` & `pyimclsts-0.1.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.5/LICENSE` & `pyimclsts-0.1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.5/README.md` & `pyimclsts-0.1.1.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,51 @@
-## PyIMCtrans
+## PyIMCLSTS
 
 This tool reads the IMC schema from a XML file, locally creates files containing the messages and connects (imports) the main global machinery.
 
 See `/example` to check an example implementation of the Follow Reference maneuver.
 
-### End-User
+### Quickstart
 - Fancying a virtual env? (Not needed. Just in case you want to isolate it from your python setup)
 ```shell
 $ sudo apt install python3.8-venv
 $ python3 -m venv tutorial_env
 $ source tutorial_env/bin/activate
 ```
 - To use:
 ```shell
 $ pip3 install pyimclsts
 $ # or, if you are cloning the repo, from the folder pyproject.toml is located:
 $ pip3 install .
+$ # If already installed, update it, with (might need to run it more than once):
+$ pip3 install -U pyimclsts
 ```
-- Choose a folder and have a version of the IMC schema. Otherwise, it will fetch the latest IMC version from the LSTS git repository. Extract messages locally, with:
+- Choose a folder and have a version of the IMC schema. Otherwise, the following command will fetch the latest IMC version from the LSTS git repository. Extract messages locally, with:
 ```shell
 $ python3 -m pyimclsts.extract
 ```
 Check how to provide a black- or whitelist using:
 ```shell
 $ python3 -m pyimclsts.extract --help
 ```
+This is unnecessary in most scenarios, but can be useful if you really have constrained resources. Use it with caution, because it may crash if, for example, you receive an inlined message that has been blacklisted.
+
 This will locally extract the IMC.xml as python classes. You will see a folder called `pyimc_generated` which contains base messages, bitfields and enumerations from the IMC.xml file. They can be locally loaded using, for example:
 ```python
 import pyimc_generated as pg
 ```
 In the top-level module, you will find some functions to allow you to connect to a vehicle and subscribe to messages, namely, a subscriber class.
 ```python
 import pyimclsts.network as n
 
 conn = n.tcp_interface('localhost', 6006)
 sub = n.subscriber(conn)
 
 # for example:
-sub.subscribe_async(myfunction, pg.messages.Announce)
+sub.subscribe_async(myfunction1, msg_id =pg.messages.Temperature, src='lauv-noptilus-1', src_ent='AHRS')
+sub.subscribe_async(myfunction2, msg_id =pg.messages.EstimatedState, src='lauv-noptilus-1', src_ent=None)
 ```
-Check `/example` for further details.
-
-### Change log:
-#### Version 0.1.1.5
-    - Fix .block_outgoing() bug
-    
-#### Version 0.1.1.4
-    - Fix extract logic bug
 
-#### Version 0.1.1.3
+In most cases, you can find the embedded documentation (docstrings) by hovering the mouse or using `help()` on interactive mode.
 
-    - Hide imports and variables of core.py
-    - Move IO interface classes to core.py
-    - Implement .block_outgoing() through an injected dependency in the message bus
-    - Improve subscriber class:
-        - Exits when Abort message is received
-        - Queries Entity List when started
-        - Tracks src and src_ent and their corresponding names
-        - Removed .subscribe_all
-            - Same functionality can be achieved with .subscribe_async()
-    
+Check `/example` for further details.
+
```

### Comparing `pyimclsts-0.1.1.5/pyproject.toml` & `pyimclsts-0.1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyimclsts"
-version = "0.1.1.5"
+version = "0.1.1.6"
 authors = [
   { name = "Choi Wang Dzak" },
 ]
 description = "Python bindings of the IMC message schema"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["IMC", "IMC message protocol", "LSTS"]
```

### Comparing `pyimclsts-0.1.1.5/PKG-INFO` & `pyimclsts-0.1.1.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimclsts
-Version: 0.1.1.5
+Version: 0.1.1.6
 Summary: Python bindings of the IMC message schema
 Project-URL: Homepage, https://github.com/choiwd/pyimctrans
 Project-URL: Bug Tracker, https://github.com/choiwd/pyimctrans/issues
 Author: Choi Wang Dzak
 License: Copyright (c) 2023 Laboratório de Sistemas e Tecnologia Subaquática
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,69 +30,58 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: ifaddr~=0.2.0
 Requires-Dist: ipaddress~=1.0.23
 Description-Content-Type: text/markdown
 
-## PyIMCtrans
+## PyIMCLSTS
 
 This tool reads the IMC schema from a XML file, locally creates files containing the messages and connects (imports) the main global machinery.
 
 See `/example` to check an example implementation of the Follow Reference maneuver.
 
-### End-User
+### Quickstart
 - Fancying a virtual env? (Not needed. Just in case you want to isolate it from your python setup)
 ```shell
 $ sudo apt install python3.8-venv
 $ python3 -m venv tutorial_env
 $ source tutorial_env/bin/activate
 ```
 - To use:
 ```shell
 $ pip3 install pyimclsts
 $ # or, if you are cloning the repo, from the folder pyproject.toml is located:
 $ pip3 install .
+$ # If already installed, update it, with (might need to run it more than once):
+$ pip3 install -U pyimclsts
 ```
-- Choose a folder and have a version of the IMC schema. Otherwise, it will fetch the latest IMC version from the LSTS git repository. Extract messages locally, with:
+- Choose a folder and have a version of the IMC schema. Otherwise, the following command will fetch the latest IMC version from the LSTS git repository. Extract messages locally, with:
 ```shell
 $ python3 -m pyimclsts.extract
 ```
 Check how to provide a black- or whitelist using:
 ```shell
 $ python3 -m pyimclsts.extract --help
 ```
+This is unnecessary in most scenarios, but can be useful if you really have constrained resources. Use it with caution, because it may crash if, for example, you receive an inlined message that has been blacklisted.
+
 This will locally extract the IMC.xml as python classes. You will see a folder called `pyimc_generated` which contains base messages, bitfields and enumerations from the IMC.xml file. They can be locally loaded using, for example:
 ```python
 import pyimc_generated as pg
 ```
 In the top-level module, you will find some functions to allow you to connect to a vehicle and subscribe to messages, namely, a subscriber class.
 ```python
 import pyimclsts.network as n
 
 conn = n.tcp_interface('localhost', 6006)
 sub = n.subscriber(conn)
 
 # for example:
-sub.subscribe_async(myfunction, pg.messages.Announce)
+sub.subscribe_async(myfunction1, msg_id =pg.messages.Temperature, src='lauv-noptilus-1', src_ent='AHRS')
+sub.subscribe_async(myfunction2, msg_id =pg.messages.EstimatedState, src='lauv-noptilus-1', src_ent=None)
 ```
-Check `/example` for further details.
-
-### Change log:
-#### Version 0.1.1.5
-    - Fix .block_outgoing() bug
-    
-#### Version 0.1.1.4
-    - Fix extract logic bug
 
-#### Version 0.1.1.3
+In most cases, you can find the embedded documentation (docstrings) by hovering the mouse or using `help()` on interactive mode.
 
-    - Hide imports and variables of core.py
-    - Move IO interface classes to core.py
-    - Implement .block_outgoing() through an injected dependency in the message bus
-    - Improve subscriber class:
-        - Exits when Abort message is received
-        - Queries Entity List when started
-        - Tracks src and src_ent and their corresponding names
-        - Removed .subscribe_all
-            - Same functionality can be achieved with .subscribe_async()
-    
+Check `/example` for further details.
+
```

