# Comparing `tmp/ipyslides-3.9.3.tar.gz` & `tmp/ipyslides-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.9.3.tar", last modified: Sun May 19 19:10:54 2024, max compression
+gzip compressed data, was "ipyslides-3.9.4.tar", last modified: Mon May 27 18:32:25 2024, max compression
```

## Comparing `ipyslides-3.9.3.tar` & `ipyslides-3.9.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 19:10:54.789558 ipyslides-3.9.3/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.9.3/LICENSE
--rw-rw-rw-   0        0        0     5382 2024-05-19 19:10:54.787565 ipyslides-3.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.9.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 19:10:54.649398 ipyslides-3.9.3/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.9.3/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-19 19:10:25.000000 ipyslides-3.9.3/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:10:54.776811 ipyslides-3.9.3/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.9.3/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    41105 2024-05-19 04:28:44.000000 ipyslides-3.9.3/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     6082 2024-05-17 21:17:49.000000 ipyslides-3.9.3/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    33033 2024-05-19 18:10:13.000000 ipyslides-3.9.3/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.9.3/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.9.3/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.9.3/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0     7884 2024-05-19 18:39:17.000000 ipyslides-3.9.3/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:10:54.783446 ipyslides-3.9.3/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    12576 2024-05-18 23:11:33.000000 ipyslides-3.9.3/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.9.3/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3563 2024-05-18 22:39:26.000000 ipyslides-3.9.3/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.9.3/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    11908 2024-05-19 16:37:54.000000 ipyslides-3.9.3/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    23555 2024-05-18 22:39:20.000000 ipyslides-3.9.3/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.9.3/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28407 2024-05-19 17:34:36.000000 ipyslides-3.9.3/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    16285 2024-05-19 17:25:46.000000 ipyslides-3.9.3/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    12668 2024-05-19 19:05:11.000000 ipyslides-3.9.3/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    47852 2024-05-19 18:00:34.000000 ipyslides-3.9.3/ipyslides/core.py
--rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.9.3/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.9.3/ipyslides/source.py
--rw-rw-rw-   0        0        0    29519 2024-05-19 18:02:34.000000 ipyslides-3.9.3/ipyslides/utils.py
--rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.9.3/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.9.3/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:10:54.727534 ipyslides-3.9.3/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5382 2024-05-19 19:10:54.000000 ipyslides-3.9.3/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-19 19:10:54.000000 ipyslides-3.9.3/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 19:10:54.000000 ipyslides-3.9.3/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-19 19:10:54.000000 ipyslides-3.9.3/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-19 19:10:54.000000 ipyslides-3.9.3/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 19:10:54.789558 ipyslides-3.9.3/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:32:25.211819 ipyslides-3.9.4/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.9.4/LICENSE
+-rw-rw-rw-   0        0        0     5382 2024-05-27 18:32:25.209809 ipyslides-3.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.9.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 18:32:25.097909 ipyslides-3.9.4/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.9.4/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-27 18:31:43.000000 ipyslides-3.9.4/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:32:25.204320 ipyslides-3.9.4/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.9.4/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    41105 2024-05-19 04:28:44.000000 ipyslides-3.9.4/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     6082 2024-05-17 21:17:49.000000 ipyslides-3.9.4/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    33033 2024-05-19 18:10:13.000000 ipyslides-3.9.4/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7547 2024-05-11 22:19:43.000000 ipyslides-3.9.4/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.9.4/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.9.4/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0     7917 2024-05-27 17:33:14.000000 ipyslides-3.9.4/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:32:25.206259 ipyslides-3.9.4/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    12576 2024-05-18 23:11:33.000000 ipyslides-3.9.4/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.9.4/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3563 2024-05-18 22:39:26.000000 ipyslides-3.9.4/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.9.4/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    11908 2024-05-19 16:37:54.000000 ipyslides-3.9.4/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    23555 2024-05-18 22:39:20.000000 ipyslides-3.9.4/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.9.4/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28407 2024-05-19 17:34:36.000000 ipyslides-3.9.4/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    16285 2024-05-19 17:25:46.000000 ipyslides-3.9.4/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    12585 2024-05-27 18:30:09.000000 ipyslides-3.9.4/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    47752 2024-05-27 17:54:56.000000 ipyslides-3.9.4/ipyslides/core.py
+-rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.9.4/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.9.4/ipyslides/source.py
+-rw-rw-rw-   0        0        0    29519 2024-05-19 18:02:34.000000 ipyslides-3.9.4/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.9.4/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.9.4/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:32:25.166148 ipyslides-3.9.4/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5382 2024-05-27 18:32:24.000000 ipyslides-3.9.4/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-27 18:32:24.000000 ipyslides-3.9.4/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 18:32:24.000000 ipyslides-3.9.4/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-27 18:32:24.000000 ipyslides-3.9.4/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-27 18:32:24.000000 ipyslides-3.9.4/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 18:32:25.211819 ipyslides-3.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.9.4/setup.py
```

### Comparing `ipyslides-3.9.3/LICENSE` & `ipyslides-3.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/PKG-INFO` & `ipyslides-3.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.9.3
+Version: 3.9.4
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.9.3/README.md` & `ipyslides-3.9.4/README.md`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_base/_layout_css.py` & `ipyslides-3.9.4/ipyslides/_base/_layout_css.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_base/_widgets.py` & `ipyslides-3.9.4/ipyslides/_base/_widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_base/base.py` & `ipyslides-3.9.4/ipyslides/_base/base.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_base/export_html.py` & `ipyslides-3.9.4/ipyslides/_base/export_html.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_base/export_template.py` & `ipyslides-3.9.4/ipyslides/_base/export_template.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_base/icons.py` & `ipyslides-3.9.4/ipyslides/_base/icons.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_base/intro.py` & `ipyslides-3.9.4/ipyslides/_base/intro.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
  +++
  more content
  ```
 ```
 
 ```python
 @slides.frames(3,*objs)
-def func(obj):
-    write(obj) #This will create as many slides after the slide number 1 as length(objs)
+def func(frame_index, frame_content):
+    write(frame_content) #This will create as many slides after the slide number 1 as length(objs)
 ```
 ```python
 slides # This displays slides if on the last line of cell, or use `slides.show()`.
 ```
 
 ::: note-info
     - You can use context managers like `with slides.slide(): ...` and `with slides.title(): ...` in place of `%%slide` and `%%title` respectively.
```

### Comparing `ipyslides-3.9.3/ipyslides/_base/js/interaction.js` & `ipyslides-3.9.4/ipyslides/_base/js/interaction.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_base/js/notes.js` & `ipyslides-3.9.4/ipyslides/_base/js/notes.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_base/navigation.py` & `ipyslides-3.9.4/ipyslides/_base/navigation.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_base/notes.py` & `ipyslides-3.9.4/ipyslides/_base/notes.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_base/screenshot.py` & `ipyslides-3.9.4/ipyslides/_base/screenshot.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_base/settings.py` & `ipyslides-3.9.4/ipyslides/_base/settings.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_base/slide.py` & `ipyslides-3.9.4/ipyslides/_base/slide.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_base/styles.py` & `ipyslides-3.9.4/ipyslides/_base/styles.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_base/widgets.py` & `ipyslides-3.9.4/ipyslides/_base/widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/_demo.py` & `ipyslides-3.9.4/ipyslides/_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     auto.from_markdown('section`Simple Animations with Frames` toc`### Contents`')
 
     forward_skipper = slides.goto_button('Skip All Next Frames')
     backward_skipper = slides.goto_button('Skip Previous Frames', icon='minus')
     
     # Animat plot in slides  
     @auto.frames(*range(14,19))
-    def func(obj,idx):
+    def func(idx, obj):
         if idx == 0:
             forward_skipper.display()
             backward_skipper.set_target()
 
         with slides.code.context(returns = True) as s:
             fig, ax = plt.subplots()
             x = np.linspace(0,obj+1,50+10*(idx+1))
@@ -198,31 +198,28 @@
             s.show_lines([5]).display()
 
     auto.from_markdown('section`Controlling Content on Frames` toc`### Contents`')
 
     # Frames structure
     boxes = [f'<div style="background:var(--hover-bg);width:auto;height:2em;padding:8px;margin:8px;border-radius:4px;"><b class="align-center">{i}</b></div>' for i in range(1,5)]
     @auto.frames(*boxes, repeat=False)
-    def f(obj,idx):
+    def f(idx, obj):
         slides.write('# Frames with \n#### `repeat = False`')
         slides.write(obj)
 
     @auto.frames(*boxes, repeat=True)
-    def f(obj,idx):
+    def f(idx, obj):
         slides.running.set_animation(None) #Disable animation for showing bullets list
         slides.write('# Frames with \n#### `repeat = True` and Fancy Bullet List')
         slides.bullets(obj, marker='💘').display()
 
     @auto.frames(*boxes, repeat=[(0,1),(2,3)])
-    def f(obj,idx):
-        with slides.code.context(returns = True) as s:
-            slides.write('# Frames with \n#### `repeat = [(0,1),(2,3)]`')
-            slides.write(*obj)
-
-        s.display()
+    def f(idx, obj):
+        slides.write('# Frames with \n#### `repeat = [(0,1),(2,3)]`')
+        slides.write(*obj)
 
     # Youtube
     from IPython.display import YouTubeVideo
     with auto.slide() as ys: # We will use this in next %%magic
         backward_skipper.display()
         forward_skipper.set_target()
         slides.format_css({'.goto-button .fa.fa-minus': slides.icon('arrow',color='crimson',rotation=180).css}).display()
```

### Comparing `ipyslides-3.9.3/ipyslides/core.py` & `ipyslides-3.9.4/ipyslides/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -721,15 +721,15 @@
             
             if len(frames) > 1 and repeat:
                 frames = ["\n".join([frames[0], *frames[1:i]]) for i in range(2, len(frames) + 1)]
             
             self._editing_index = None
             
             @self.frames(int(slide_number_str), *frames, repeat=False) # here repeat handled above
-            def make_slide(frm, idx):
+            def make_slide(idx, frm):
                 if (self.running.markdown != frm) or (idx == 0):
                     self._editing_index = self.running.index # Go to latest editing markdown frame, or start of frames
 
                 self.running.set_source(frm, "markdown")  # Update source beofore parsing content to make it available to user inside markdown too
                 parse(xtr.copy_ns(cell, frm), returns = False)
             
             if self._editing_index is not None:
@@ -818,25 +818,25 @@
                     else:
                         slide._slide_tocbox.remove_class("FirstTOC")
         
         self.notify('Dynamic content updated everywhere!')
                 
 
     def frames(self, slide_number, *objs, repeat=False):
-        """Decorator for inserting frames on slide, define a function with two arguments acting on each obj in objs and current frame index.
-        You can also call it as a function, e.g. `.frames(1,*objs)()` becuase it can write by defualt.
+        """Decorator for inserting frames on slide, define a function with two arguments (frame_index, frame_content).
+        You can also call it as a function, e.g. `.frames(1,*objs)(<optional function>)`.
 
         ```python
         @slides.frames(1,a,b,c) # slides 1.1, 1.2, 1.3 with content a,b,c
-        def f(obj, idx):
-            do_something(obj)
-            if idx == 0: # Main Slide
+        def f(frame_index, frame_content):
+            do_something(frame_content)
+            if frame_index == 0: # Main Slide
                 print('This is main slide')
             else:
-                print('This is frame', idx)
+                print('This is frame', frame_index)
 
         slides.frames(1,a,b,c)() # Auto writes the frames with same content as above
         slides.frames(1,a,b,c, repeat = True)() # content is [a], [a,b], [a,b,c] from top to bottom
         slides.frames(1,a,b,c, repeat = [(0,1),(1,2)])() # two frames with content [a,b] and [b,c]
         ```
 
         **Parameters**
@@ -844,20 +844,17 @@
         - slide_number: (int) slide number to insert frames on.
         - objs: expanded by * (list, tuple) of objects to write on frames. If repeat is False, only one frame is generated for each obj.
         - repeat: (bool, list, tuple) If False, only one frame is generated for each obj.
             If True, one frame are generated in sequence of ojects linke `[a,b,c]` will generate 3 frames with [a], [a,b], [a,b,c] to given in function and will be written top to bottom.
             If list or tuple, it will be used as the sequence of frames to generate and number of frames = len(repeat).
             [(0,1),(1,2)] will generate 2 frames with [a,b] and [b,c] to given in function and will be written top to bottom or the way you write in your function.
         
-        No return of defined function required, if any, only should be display/show etc.
-        CSS properties from `prop_dict` are applied to all slides from *objs."""
+        No return of defined function required, if any, only should be display/show etc."""
 
-        def _frames(
-            func=lambda obj, idx: self.write(obj)
-        ):  # default write if called without function
+        def _frames(func = lambda idx, obj: self.write(obj)):  # write if called without function
             if not isinstance(slide_number, int):
                 return print(f"slide_number expects integer, got {slide_number!r}")
 
             if slide_number < 0:  # title slide is 0
                 raise ValueError(f"slide_number should be >= 1, got {slide_number!r}")
 
             if repeat == True:
@@ -878,15 +875,15 @@
                     f"Maximum 99 frames are supported, found {len(_new_objs)} frames!"
                 )
 
             # build_slide returns old slide with updated display if exists.
             with _build_slide(
                 self, f"{slide_number}", is_frameless=False
             ) as this_slide:
-                func(_new_objs[0], 0)  # Main slide content
+                func(0, _new_objs[0])  # Main slide content
 
             _new_objs = _new_objs[1:]  # Fisrt one is already written
 
             NFRAMES_OLD = len(this_slide._frames)  # old frames
 
             new_frames = []
             for i, obj in enumerate(_new_objs):  # New frames
@@ -895,15 +892,15 @@
                 else:  # Update old frames
                     new_slide = this_slide._frames[i]  # Take same frame back
                     new_slide.reset_source() # Reset old source but keep markdown for observing edits
 
                 new_frames.append(new_slide)
 
                 with new_slide._capture() as captured:
-                    func(obj, i + 1)  # i+1 as main slide is 0
+                    func(i + 1, obj)  # i+1 as main slide is 0
 
             this_slide._frames = new_frames
 
             if len(this_slide._frames) != NFRAMES_OLD:
                 this_slide._rebuild_all()  # Rebuild all slides as frames changed
 
             # Update All displays
```

### Comparing `ipyslides-3.9.3/ipyslides/formatters.py` & `ipyslides-3.9.4/ipyslides/formatters.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/source.py` & `ipyslides-3.9.4/ipyslides/source.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/utils.py` & `ipyslides-3.9.4/ipyslides/utils.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/writer.py` & `ipyslides-3.9.4/ipyslides/writer.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides/xmd.py` & `ipyslides-3.9.4/ipyslides/xmd.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/ipyslides.egg-info/PKG-INFO` & `ipyslides-3.9.4/ipyslides.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.9.3
+Version: 3.9.4
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.9.3/ipyslides.egg-info/SOURCES.txt` & `ipyslides-3.9.4/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.3/setup.py` & `ipyslides-3.9.4/setup.py`

 * *Files identical despite different names*

