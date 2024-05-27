# Comparing `tmp/pymupdf4llm-0.0.3.tar.gz` & `tmp/pymupdf4llm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymupdf4llm-0.0.3.tar", last modified: Tue May 21 01:56:27 2024, max compression
+gzip compressed data, was "pymupdf4llm-0.0.4.tar", last modified: Mon May 27 09:37:57 2024, max compression
```

## Comparing `pymupdf4llm-0.0.3.tar` & `pymupdf4llm-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 01:56:27.190764 pymupdf4llm-0.0.3/
--rw-rw-rw-   0        0        0     3855 2024-05-21 01:56:27.189765 pymupdf4llm-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3337 2024-05-20 17:05:17.000000 pymupdf4llm-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 01:56:27.153776 pymupdf4llm-0.0.3/pymupdf4llm/
--rw-rw-rw-   0        0        0      324 2024-05-20 23:55:29.000000 pymupdf4llm-0.0.3/pymupdf4llm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 01:56:27.180760 pymupdf4llm-0.0.3/pymupdf4llm/helpers/
--rw-rw-rw-   0        0        0     7876 2024-05-21 00:05:21.000000 pymupdf4llm-0.0.3/pymupdf4llm/helpers/get_text_lines.py
--rw-rw-rw-   0        0        0    12609 2024-05-21 00:06:41.000000 pymupdf4llm-0.0.3/pymupdf4llm/helpers/multi_column.py
--rw-rw-rw-   0        0        0    19201 2024-05-21 01:52:20.000000 pymupdf4llm-0.0.3/pymupdf4llm/helpers/pymupdf_rag.py
-drwxrwxrwx   0        0        0        0 2024-05-21 01:56:27.187768 pymupdf4llm-0.0.3/pymupdf4llm/llama/
--rw-rw-rw-   0        0        0     5040 2024-05-20 23:09:59.000000 pymupdf4llm-0.0.3/pymupdf4llm/llama/pdf_markdown_reader.py
-drwxrwxrwx   0        0        0        0 2024-05-21 01:56:27.188761 pymupdf4llm-0.0.3/pymupdf4llm.egg-info/
--rw-rw-rw-   0        0        0     3855 2024-05-21 01:56:27.000000 pymupdf4llm-0.0.3/pymupdf4llm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2024-05-21 01:56:27.000000 pymupdf4llm-0.0.3/pymupdf4llm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 01:56:27.000000 pymupdf4llm-0.0.3/pymupdf4llm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-21 01:56:27.000000 pymupdf4llm-0.0.3/pymupdf4llm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 01:56:27.000000 pymupdf4llm-0.0.3/pymupdf4llm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 01:56:27.190764 pymupdf4llm-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      989 2024-05-20 23:51:52.000000 pymupdf4llm-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:37:57.103090 pymupdf4llm-0.0.4/
+-rw-rw-rw-   0        0        0     3855 2024-05-27 09:37:57.102179 pymupdf4llm-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3337 2024-05-20 17:05:17.000000 pymupdf4llm-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 09:37:57.050430 pymupdf4llm-0.0.4/pymupdf4llm/
+-rw-rw-rw-   0        0        0      324 2024-05-20 23:55:29.000000 pymupdf4llm-0.0.4/pymupdf4llm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:37:57.092480 pymupdf4llm-0.0.4/pymupdf4llm/helpers/
+-rw-rw-rw-   0        0        0     7876 2024-05-21 00:05:21.000000 pymupdf4llm-0.0.4/pymupdf4llm/helpers/get_text_lines.py
+-rw-rw-rw-   0        0        0    12609 2024-05-21 00:06:41.000000 pymupdf4llm-0.0.4/pymupdf4llm/helpers/multi_column.py
+-rw-rw-rw-   0        0        0    22421 2024-05-27 09:12:57.000000 pymupdf4llm-0.0.4/pymupdf4llm/helpers/pymupdf_rag.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:37:57.100089 pymupdf4llm-0.0.4/pymupdf4llm/llama/
+-rw-rw-rw-   0        0        0     3423 2024-05-23 22:35:17.000000 pymupdf4llm-0.0.4/pymupdf4llm/llama/pdf_markdown_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:37:57.101168 pymupdf4llm-0.0.4/pymupdf4llm.egg-info/
+-rw-rw-rw-   0        0        0     3855 2024-05-27 09:37:57.000000 pymupdf4llm-0.0.4/pymupdf4llm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2024-05-27 09:37:57.000000 pymupdf4llm-0.0.4/pymupdf4llm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 09:37:57.000000 pymupdf4llm-0.0.4/pymupdf4llm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 09:37:57.000000 pymupdf4llm-0.0.4/pymupdf4llm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-27 09:37:57.000000 pymupdf4llm-0.0.4/pymupdf4llm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 09:37:57.103090 pymupdf4llm-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      989 2024-05-27 09:37:12.000000 pymupdf4llm-0.0.4/setup.py
```

### Comparing `pymupdf4llm-0.0.3/PKG-INFO` & `pymupdf4llm-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymupdf4llm
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyMuPDF Utilities for LLM/RAG
 Home-page: https://github.com/pymupdf/RAG
 Author: Artifex
 Author-email: support@artifex.com
 License: GNU AFFERO GPL 3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pymupdf4llm-0.0.3/README.md` & `pymupdf4llm-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pymupdf4llm-0.0.3/pymupdf4llm/helpers/get_text_lines.py` & `pymupdf4llm-0.0.4/pymupdf4llm/helpers/get_text_lines.py`

 * *Files identical despite different names*

### Comparing `pymupdf4llm-0.0.3/pymupdf4llm/helpers/multi_column.py` & `pymupdf4llm-0.0.4/pymupdf4llm/helpers/multi_column.py`

 * *Files identical despite different names*

### Comparing `pymupdf4llm-0.0.3/pymupdf4llm/helpers/pymupdf_rag.py` & `pymupdf4llm-0.0.4/pymupdf4llm/helpers/pymupdf_rag.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,22 +36,27 @@
 
 from pymupdf4llm.helpers.get_text_lines import get_raw_lines, is_white
 from pymupdf4llm.helpers.multi_column import column_boxes
 
 if fitz.pymupdf_version_tuple < (1, 24, 2):
     raise NotImplementedError("PyMuPDF version 1.24.2 or later is needed.")
 
-bullet = ("* ", chr(0xF0B7), chr(0xB7), chr(8226), chr(9679))
+bullet = ("- ", "* ", chr(0xF0A7), chr(0xF0B7), chr(0xB7), chr(8226), chr(9679))
 GRAPHICS_TEXT = "\n![%s](%s)\n"
 
 
 class IdentifyHeaders:
     """Compute data for identifying header text."""
 
-    def __init__(self, doc, pages: list = None, body_limit: float = None):
+    def __init__(
+        self,
+        doc: str,
+        pages: list = None,
+        body_limit: float = 12,
+    ):
         """Read all text and make a dictionary of fontsizes.
 
         Args:
             pages: optional list of pages to consider
             body_limit: consider text with larger font size as some header
         """
         if isinstance(doc, fitz.Document):
@@ -81,96 +86,114 @@
             # if opened here, close it now
             mydoc.close()
 
         # maps a fontsize to a string of multiple # header tag characters
         self.header_id = {}
 
         # If not provided, choose the most frequent font size as body text.
-        # If no text at all on all pages, just use 12
-        if body_limit is None:
-            temp = sorted(
-                [(k, v) for k, v in fontsizes.items()],
-                key=lambda i: i[1],
-                reverse=True,
-            )
-            if temp:
-                body_limit = temp[0][0]
-            else:
-                body_limit = 12
+        # If no text at all on all pages, just use 12.
+        # In any case all fonts not exceeding
+        temp = sorted(
+            [(k, v) for k, v in fontsizes.items()],
+            key=lambda i: i[1],
+            reverse=True,
+        )
+        if temp:
+            b_limit = max(body_limit, temp[0][0])
+        else:
+            b_limit = body_limit
 
-        sizes = sorted([f for f in fontsizes.keys() if f > body_limit], reverse=True)
+        # identify up to 6 font sizes as header candidates
+        sizes = sorted(
+            [f for f in fontsizes.keys() if f > b_limit],
+            reverse=True,
+        )[:6]
 
         # make the header tag dictionary
         for i, size in enumerate(sizes):
             self.header_id[size] = "#" * (i + 1) + " "
 
-    def get_header_id(self, span):
+    def get_header_id(self, span: dict, page=None) -> str:
         """Return appropriate markdown header prefix.
 
-        Given a text span from a "dict"/"radict" extraction, determine the
-        markdown header prefix string of 0 to many concatenated '#' characters.
+        Given a text span from a "dict"/"rawdict" extraction, determine the
+        markdown header prefix string of 0 to n concatenated '#' characters.
         """
         fontsize = round(span["size"])  # compute fontsize
         hdr_id = self.header_id.get(fontsize, "")
         return hdr_id
 
 
 def to_markdown(
-    doc: fitz.Document | str,
+    doc: str,
     *,
-    pages: list | range | None = None,
-    hdr_info: IdentifyHeaders | None = None,
+    pages: list = None,
+    hdr_info=None,
     write_images: bool = False,
     page_chunks: bool = False,
-) -> str | list[dict]:
+    margins: typing.Iterable = (0, 50, 0, 50),
+) -> str:
     """Process the document and return the text of its selected pages."""
 
     if isinstance(doc, str):
         doc = fitz.open(doc)
 
-    if not pages:  # use all pages if argument not given
-        pages = range(doc.page_count)
+    if pages is None:  # use all pages if no selection given
+        pages = list(range(doc.page_count))
 
-    if not isinstance(hdr_info, IdentifyHeaders):
+    if hasattr(margins, "__float__"):
+        margins = [margins] * 4
+    if len(margins) == 2:
+        margins = (0, margins[0], 0, margins[1])
+    if len(margins) != 4:
+        raise ValueError("margins must have length 2 or 4 or be a number.")
+    elif not all([hasattr(m, "__float__") for m in margins]):
+        raise ValueError("margin values must be numbers")
+
+    # If "hdr_info" is not an object having method "get_header_id", scan the
+    # document and use font sizes as header level indicators.
+    if callable(hdr_info):
+        get_header_id = hdr_info
+    elif hasattr(hdr_info, "get_header_id") and callable(hdr_info.get_header_id):
+        get_header_id = hdr_info.get_header_id
+    else:
         hdr_info = IdentifyHeaders(doc)
+        get_header_id = hdr_info.get_header_id
 
     def resolve_links(links, span):
         """Accept a span and return a markdown link string."""
         bbox = fitz.Rect(span["bbox"])  # span bbox
         # a link should overlap at least 70% of the span
         bbox_area = 0.7 * abs(bbox)
         for link in links:
             hot = link["from"]  # the hot area of the link
             if not abs(hot & bbox) >= bbox_area:
                 continue  # does not touch the bbox
             text = f'[{span["text"].strip()}]({link["uri"]})'
             return text
 
     def save_image(page, rect, i):
-        """Optionally render the rect part of a page.
-
-        In any case return the image filename.
-        """
+        """Optionally render the rect part of a page."""
         filename = page.parent.name.replace("\\", "/")
         image_path = f"{filename}-{page.number}-{i}.png"
         if write_images is True:
             pix = page.get_pixmap(clip=rect)
             pix.save(image_path)
             del pix
-        return os.path.basename(image_path)
+            return os.path.basename(image_path)
+        return ""
 
     def write_text(
         page: fitz.Page,
         textpage: fitz.TextPage,
         clip: fitz.Rect,
         tabs=None,
-        tab_rects: dict | None = None,
-        img_rects: dict | None = None,
-        links: list | None = None,
-        hdr_info=None,
+        tab_rects: dict = None,
+        img_rects: dict = None,
+        links: list = None,
     ) -> string:
         """Output the text found inside the given clip.
 
         This is an alternative for plain text in that it outputs
         text enriched with markdown styling.
         The logic is capable of recognizing headers, body text, code blocks,
         inline code, bold, italic and bold-italic styling.
@@ -223,15 +246,16 @@
                     j
                     for j in img_rects.items()
                     if j[1].y1 <= lrect.y0 and not (j[1] & clip).is_empty
                 ],
                 key=lambda j: (j[1].y1, j[1].x0),
             ):
                 pathname = save_image(page, img_rect, i)
-                out_string += GRAPHICS_TEXT % (pathname, pathname)
+                if pathname:
+                    out_string += GRAPHICS_TEXT % (pathname, pathname)
                 del img_rects[i]
 
             text = " ".join([s["text"] for s in spans])
 
             # if the full line mono-spaced?
             all_mono = all([s["flags"] & 8 for s in spans])
 
@@ -243,44 +267,49 @@
                 # of 0.5*fontsize.
                 delta = int((lrect.x0 - clip.x0) / (spans[0]["size"] * 0.5))
                 indent = " " * delta
 
                 out_string += indent + text + "\n"
                 continue  # done with this line
 
-            bno = spans[0]["block"]  # block number of line
+            span0 = spans[0]
+            bno = span0["block"]  # block number of line
             if bno != prev_bno:
                 out_string += "\n"
                 prev_bno = bno
-            span0 = spans[0]
 
             if (  # check if we need another line break
                 prev_lrect
                 and lrect.y1 - prev_lrect.y1 > lrect.height * 1.5
                 or span0["text"].startswith("[")
                 or span0["text"].startswith(bullet)
                 or span0["flags"] & 1  # superscript?
             ):
                 out_string += "\n"
             prev_lrect = lrect
 
             # if line is a header, this will return multiple "#" characters
-            hdr_string = hdr_info.get_header_id(spans[0])
+            hdr_string = get_header_id(span0, page=page)
 
             # intercept if header text has been broken in multiple lines
             if hdr_string and hdr_string == prev_hdr_string:
                 out_string = out_string[:-1] + " " + text + "\n"
                 continue
+
             prev_hdr_string = hdr_string
+            if hdr_string.startswith("#"):  # if a header line skip the rest
+                out_string += hdr_string + text + "\n"
+                continue
+
+            # this line is not all-mono, so switch off "code" mode
+            if code:  # still in code output mode?
+                out_string += "```\n"  # switch of code mode
+                code = False
 
             for i, s in enumerate(spans):  # iterate spans of the line
-                # this line is not all-mono, so switch off "code" mode
-                if code:  # still in code output mode?
-                    out_string += "```\n"  # switch of code mode
-                    code = False
                 # decode font properties
                 mono = s["flags"] & 8
                 bold = s["flags"] & 16
                 italic = s["flags"] & 2
 
                 if mono:
                     # this is text in some monospaced font
@@ -308,14 +337,15 @@
                     out_string += text
             if not code:
                 out_string += "\n"
         out_string += "\n"
         if code:
             out_string += "```\n"  # switch of code mode
             code = False
+
         return (
             out_string.replace(" \n", "\n").replace("  ", " ").replace("\n\n\n", "\n\n")
         )
 
     def is_in_rects(rect, rect_list):
         """Check if rect is contained in a rect of the list."""
         for i, r in enumerate(rect_list, start=1):
@@ -357,76 +387,123 @@
         this_md = ""  # markdown string
         if text_rect is not None:  # select tables above the text block
             for i, img_rect in sorted(
                 [j for j in img_rects.items() if j[1].y1 <= text_rect.y0],
                 key=lambda j: (j[1].y1, j[1].x0),
             ):
                 pathname = save_image(page, img_rect, i)
-                this_md += GRAPHICS_TEXT % (pathname, pathname)
+                if pathname:
+                    this_md += GRAPHICS_TEXT % (pathname, pathname)
                 del img_rects[i]  # do not touch this image twice
 
         else:  # output all remaining table
             for i, img_rect in sorted(
                 img_rects.items(),
                 key=lambda j: (j[1].y1, j[1].x0),
             ):
                 pathname = save_image(page, img_rect, i)
-                this_md += GRAPHICS_TEXT % (pathname, pathname)
+                if pathname:
+                    this_md += GRAPHICS_TEXT % (pathname, pathname)
                 del img_rects[i]  # do not touch this image twice
         return this_md
 
     def get_metadata(doc, pno):
         meta = doc.metadata.copy()
         meta["file_path"] = doc.name
         meta["page_count"] = doc.page_count
         meta["page"] = pno + 1
         return meta
 
-    def get_page_output(doc, pno, textflags):
-        """Process one page."""
+    def get_page_output(doc, pno, margins, textflags):
+        """Process one page.
+
+        Args:
+            doc: fitz.Document
+            pno: 0-based page number
+            textflags: text extraction flag bits
+
+        Returns:
+            Markdown string of page content and image, table and vector
+            graphics information.
+        """
         page = doc[pno]
         md_string = ""
-
+        left, top, right, bottom = margins
+        clip = page.rect + (left, top, -right, -bottom)
         # extract all links on page
         links = [l for l in page.get_links() if l["kind"] == 2]
 
         # make a TextPage for all later extractions
-        textpage = page.get_textpage(flags=textflags)
+        textpage = page.get_textpage(flags=textflags, clip=clip)
+
+        img_info = [img for img in page.get_image_info() if img["bbox"] in clip]
+        images = img_info[:]
+        tables = []
+        graphics = []
 
         # Locate all tables on page
-        tabs = page.find_tables()
+        tabs = page.find_tables(clip=clip, strategy="lines_strict")
 
         # Make a list of table boundary boxes.
         # Must include the header bbox (may exist outside tab.bbox)
         tab_rects = {}
         for i, t in enumerate(tabs):
             tab_rects[i] = fitz.Rect(t.bbox) | fitz.Rect(t.header.bbox)
+            tab_dict = {
+                "bbox": tuple(tab_rects[i]),
+                "rows": t.row_count,
+                "columns": t.col_count,
+            }
+            tables.append(tab_dict)
         tab_rects0 = list(tab_rects.values())
 
         # Select paths that are not contained in any table
         page_clip = page.rect + (36, 36, -36, -36)  # ignore full page graphics
         paths = [
             p
             for p in page.get_drawings()
-            if not intersects_rects(p["rect"], tab_rects0) and p["rect"] in page_clip
+            if not intersects_rects(p["rect"], tab_rects0)
+            and p["rect"] in page_clip
+            and p["rect"].width < page_clip.width
+            and p["rect"].height < page_clip.height
         ]
 
-        # determine vector graphics outside any tables
-        vg_clusters = page.cluster_drawings(drawings=paths)
+        # Determine vector graphics outside any tables, filerting out any
+        # which contain no stroked paths
+        vg_clusters = []
+        for bbox in page.cluster_drawings(drawings=paths):
+            include = False
+            for p in [p for p in paths if p["rect"] in bbox]:
+                if p["type"] != "f":
+                    include = True
+                    break
+                if [item[0] for item in p["items"] if item[0] == "c"]:
+                    include = True
+                    break
+                if include is True:
+                    vg_clusters.append(bbox)
+
+        actual_paths = [p for p in paths if is_in_rects(p["rect"], vg_clusters)]
+
         vg_clusters0 = [
             r
             for r in vg_clusters
             if not intersects_rects(r, tab_rects0) and r.height > 20
-        ] + [fitz.Rect(i["bbox"]) for i in page.get_image_info()]
+        ]
+
+        if write_images is True:
+            vg_clusters0 += [fitz.Rect(i["bbox"]) for i in img_info]
 
         vg_clusters = dict((i, r) for i, r in enumerate(vg_clusters0))
+
         # Determine text column bboxes on page, avoiding tables and graphics
         text_rects = column_boxes(
             page,
-            paths=paths,
+            paths=actual_paths,
+            no_image_text=write_images,
             textpage=textpage,
             avoid=tab_rects0 + vg_clusters0,
         )
         """Extract markdown text iterating over text rectangles.
         We also output any tables. They may live above, below or inside
         the text rectangles.
         """
@@ -440,36 +517,54 @@
                 page,
                 textpage,
                 text_rect,
                 tabs=tabs,
                 tab_rects=tab_rects,
                 img_rects=vg_clusters,
                 links=links,
-                hdr_info=hdr_info,
             )
 
-        # write remaining tables.
+        # write any remaining tables and images
         md_string += output_tables(tabs, None, tab_rects)
         md_string += output_images(None, tab_rects, None)
         md_string += "\n-----\n\n"
-        return md_string
+        while md_string.startswith("\n"):
+            md_string = md_string[1:]
+        return md_string, images, tables, graphics
 
     if page_chunks is False:
         document_output = ""
     else:
         document_output = []
 
+    # read the Table of Contents
+    toc = doc.get_toc()
     textflags = fitz.TEXT_DEHYPHENATE | fitz.TEXT_MEDIABOX_CLIP
-    for pno in list(pages):
-        page_output = get_page_output(doc, pno, textflags)
+    for pno in pages:
+
+        page_output, images, tables, graphics = get_page_output(
+            doc, pno, margins, textflags
+        )
         if page_chunks is False:
             document_output += page_output
         else:
+            # build subet of TOC for this page
+            page_tocs = [t for t in toc if t[-1] == pno + 1]
+
             metadata = get_metadata(doc, pno)
-            document_output.append({"metadata": metadata, "text": page_output})
+            document_output.append(
+                {
+                    "metadata": metadata,
+                    "toc_items": page_tocs,
+                    "tables": tables,
+                    "images": images,
+                    "graphics": graphics,
+                    "text": page_output,
+                }
+            )
 
     return document_output
 
 
 if __name__ == "__main__":
     import pathlib
     import sys
```

### Comparing `pymupdf4llm-0.0.3/pymupdf4llm/llama/pdf_markdown_reader.py` & `pymupdf4llm-0.0.4/pymupdf4llm/llama/pdf_markdown_reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Union
 
 try:
     import pymupdf as fitz  # available with v1.24.3
 except ImportError:
     import fitz
@@ -19,23 +18,20 @@
 except ImportError:
     raise NotImplementedError("Please install required 'llama_index'.")
 
 
 class PDFMarkdownReader(BaseReader):
     """Read PDF files using PyMuPDF library."""
 
-    use_doc_meta: bool = True
     meta_filter: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None
 
     def __init__(
         self,
-        use_doc_meta: bool = True,
         meta_filter: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
     ):
-        self.use_doc_meta = use_doc_meta
         self.meta_filter = meta_filter
 
     def load_data(
         self,
         file_path: Union[Path, str],
         extra_info: Optional[Dict] = None,
         **load_kwargs: Any,
@@ -69,67 +65,27 @@
             docs.append(
                 self._process_doc_page(
                     doc, extra_info, file_path, page.number, hdr_info
                 )
             )
         return docs
 
-    async def aload_data(
-        self,
-        file_path: Union[Path, str],
-        extra_info: Optional[Dict] = None,
-        **load_kwargs: Any,
-    ) -> List[LlamaIndexDocument]:
-        """Asynchronously loads list of documents from PDF file and also accepts extra information in dict format.
-
-        Args:
-            file_path (Union[Path, str]): The path to the PDF file.
-            extra_info (Optional[Dict], optional): A dictionary containing extra information. Defaults to None.
-            **load_kwargs (Any): Additional keyword arguments to be passed to the load method.
-
-        Returns:
-            List[LlamaIndexDocument]: A list of LlamaIndexDocument objects.
-        """
-        if not isinstance(file_path, str) and not isinstance(file_path, Path):
-            raise TypeError("file_path must be a string or Path.")
-
-        if not extra_info:
-            extra_info = {}
-
-        if extra_info and not isinstance(extra_info, dict):
-            raise TypeError("extra_info must be a dictionary.")
-
-        # extract text header information
-        hdr_info = IdentifyHeaders(file_path)
-
-        doc: FitzDocument = fitz.open(file_path)
-        tasks = []
-
-        for page in doc:
-            tasks.append(
-                self._process_doc_page(
-                    doc, extra_info, file_path, page.number, hdr_info
-                )
-            )
-        return await asyncio.gather(*tasks)
-
     # Helpers
     # ---
 
     def _process_doc_page(
         self,
         doc: FitzDocument,
         extra_info: Dict[str, Any],
         file_path: str,
         page_number: int,
         hdr_info: IdentifyHeaders,
     ):
         """Processes a single page of a PDF document."""
-        if self.use_doc_meta:
-            extra_info = self._process_doc_meta(doc, file_path, page_number, extra_info)
+        extra_info = self._process_doc_meta(doc, file_path, page_number, extra_info)
 
         if self.meta_filter:
             extra_info = self.meta_filter(extra_info)
 
         text = to_markdown(
             doc, pages=[page_number], hdr_info=hdr_info, write_images=False
         )
```

### Comparing `pymupdf4llm-0.0.3/pymupdf4llm.egg-info/PKG-INFO` & `pymupdf4llm-0.0.4/pymupdf4llm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymupdf4llm
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyMuPDF Utilities for LLM/RAG
 Home-page: https://github.com/pymupdf/RAG
 Author: Artifex
 Author-email: support@artifex.com
 License: GNU AFFERO GPL 3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pymupdf4llm-0.0.3/setup.py` & `pymupdf4llm-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "Programming Language :: Python :: 3",
     "Topic :: Utilities",
 ]
 requires = ["pymupdf>=1.24.2"]
 
 setuptools.setup(
     name="pymupdf4llm",
-    version="0.0.3",
+    version="0.0.4",
     author="Artifex",
     author_email="support@artifex.com",
     description="PyMuPDF Utilities for LLM/RAG",
     packages=setuptools.find_packages(),
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requires,
```

