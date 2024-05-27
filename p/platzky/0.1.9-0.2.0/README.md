# Comparing `tmp/platzky-0.1.9.tar.gz` & `tmp/platzky-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platzky-0.1.9.tar", max compression
+gzip compressed data, was "platzky-0.2.0.tar", max compression
```

## Comparing `platzky-0.1.9.tar` & `platzky-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,34 @@
--rw-r--r--   0        0        0       34 2022-10-17 00:54:36.648188 platzky-0.1.9/README.md
--rw-r--r--   0        0        0        0 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/__init__.py
--rw-r--r--   0        0        0     2361 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/blog/blog.py
--rw-r--r--   0        0        0      467 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/blog/comment_form.py
--rw-r--r--   0        0        0      315 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/blog/db.py
--rw-r--r--   0        0        0      456 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/blog/post_formatter.py
--rw-r--r--   0        0        0     1090 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/config.py
--rw-r--r--   0        0        0     5088 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/db/__pycache__/graphQl.cpython-310.pyc
--rw-r--r--   0        0        0     4761 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/db/graphQl.py
--rw-r--r--   0        0        0     1764 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/db/json_file.py
--rw-r--r--   0        0        0      437 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/db_loader.py
--rw-r--r--   0        0        0     2757 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/platzky.py
--rw-r--r--   0        0        0      750 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/plugin_loader.py
--rw-r--r--   0        0        0     1003 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/plugins/redirections/entrypoint.py
--rw-r--r--   0        0        0     2500 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/seo/seo.py
--rw-r--r--   0        0        0     8082 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/static/blog.css
--rw-r--r--   0        0        0       78 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/templates/404.html
--rw-r--r--   0        0        0     1944 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/templates/base.html
--rw-r--r--   0        0        0     1219 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/templates/blog.html
--rw-r--r--   0        0        0     1141 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/templates/body_meta.html
--rw-r--r--   0        0        0      854 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/templates/feed.xml
--rw-r--r--   0        0        0     1782 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/templates/head_meta.html
--rw-r--r--   0        0        0     3900 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/templates/home.html
--rw-r--r--   0        0        0      655 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/templates/page.html
--rw-r--r--   0        0        0     1906 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/templates/post.html
--rw-r--r--   0        0        0      116 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/templates/robots.txt
--rw-r--r--   0        0        0      578 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/templates/sitemap.xml
--rw-r--r--   0        0        0      688 2022-10-17 00:54:36.648188 platzky-0.1.9/platzky/www_handler.py
--rw-r--r--   0        0        0      522 2022-10-17 00:54:36.652188 platzky-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 platzky-0.1.9/setup.py
--rw-r--r--   0        0        0      764 1970-01-01 00:00:00.000000 platzky-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      768 2024-05-27 15:15:03.928634 platzky-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/blog/__init__.py
+-rw-r--r--   0        0        0     3031 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/blog/blog.py
+-rw-r--r--   0        0        0      513 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/blog/comment_form.py
+-rw-r--r--   0        0        0     2203 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/config.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/db/__init__.py
+-rw-r--r--   0        0        0     2876 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/db/db.py
+-rw-r--r--   0        0        0      905 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/db/db_loader.py
+-rw-r--r--   0        0        0     1513 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/db/google_json_db.py
+-rw-r--r--   0        0        0     6974 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/db/graph_ql_db.py
+-rw-r--r--   0        0        0     3328 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/db/json_db.py
+-rw-r--r--   0        0        0     1010 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/db/json_file_db.py
+-rw-r--r--   0        0        0     1450 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/models.py
+-rw-r--r--   0        0        0     4649 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/platzky.py
+-rw-r--r--   0        0        0     1106 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/plugin_loader.py
+-rw-r--r--   0        0        0     1565 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/plugins/redirections/entrypoint.py
+-rw-r--r--   0        0        0     1237 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/plugins/sendmail/entrypoint.py
+-rw-r--r--   0        0        0     2710 2024-05-27 15:15:03.928634 platzky-0.2.0/platzky/seo/seo.py
+-rw-r--r--   0        0        0     7895 2024-05-27 15:15:03.932634 platzky-0.2.0/platzky/static/blog.css
+-rw-r--r--   0        0        0       78 2024-05-27 15:15:03.932634 platzky-0.2.0/platzky/templates/404.html
+-rw-r--r--   0        0        0     4966 2024-05-27 15:15:03.932634 platzky-0.2.0/platzky/templates/base.html
+-rw-r--r--   0        0        0     1281 2024-05-27 15:15:03.932634 platzky-0.2.0/platzky/templates/blog.html
+-rw-r--r--   0        0        0      526 2024-05-27 15:15:03.932634 platzky-0.2.0/platzky/templates/body_meta.html
+-rw-r--r--   0        0        0      863 2024-05-27 15:15:03.932634 platzky-0.2.0/platzky/templates/feed.xml
+-rw-r--r--   0        0        0     1370 2024-05-27 15:15:03.932634 platzky-0.2.0/platzky/templates/head_meta.html
+-rw-r--r--   0        0        0     3900 2024-05-27 15:15:03.932634 platzky-0.2.0/platzky/templates/home.html
+-rw-r--r--   0        0        0      647 2024-05-27 15:15:03.932634 platzky-0.2.0/platzky/templates/page.html
+-rw-r--r--   0        0        0     1906 2024-05-27 15:15:03.932634 platzky-0.2.0/platzky/templates/post.html
+-rw-r--r--   0        0        0      116 2024-05-27 15:15:03.932634 platzky-0.2.0/platzky/templates/robots.txt
+-rw-r--r--   0        0        0      578 2024-05-27 15:15:03.932634 platzky-0.2.0/platzky/templates/sitemap.xml
+-rw-r--r--   0        0        0      725 2024-05-27 15:15:03.932634 platzky-0.2.0/platzky/www_handler.py
+-rw-r--r--   0        0        0      841 2024-05-27 15:15:03.932634 platzky-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1550 1970-01-01 00:00:00.000000 platzky-0.2.0/PKG-INFO
```

### Comparing `platzky-0.1.9/platzky/seo/seo.py` & `platzky-0.2.0/platzky/seo/seo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,77 @@
+import typing as t
 import urllib.parse
-from flask import request, render_template, make_response, Blueprint
+from os.path import dirname
+from flask import Blueprint, current_app, make_response, render_template, request
 
 
-def create_seo_blueprint(db, config):
-    url_prefix = config["SEO_PREFIX"]
-    seo = Blueprint('seo', __name__, url_prefix=url_prefix)
-    languages = config["LANG_MAP"]
-    main_domain = config["MAIN_DOMAIN"]
-    # secure_headers = SecureHeaders()
+def create_seo_blueprint(db, config: dict[str, t.Any]):
+    seo = Blueprint(
+        "seo",
+        __name__,
+        url_prefix=config["SEO_PREFIX"],
+        template_folder=f"{dirname(__file__)}/../templates",
+    )
 
     @seo.route("/robots.txt")
     def robots():
-        robots_response = render_template("robots.txt", domain=request.host, mimetype='text/plain')
+        robots_response = render_template(
+            "robots.txt", domain=request.host, mimetype="text/plain"
+        )
         response = make_response(robots_response)
         response.headers["Content-Type"] = "text/plain"
         return response
 
-    @seo.route("/sitemap.xml", host=languages['pl']['domain'])
-    def pl_sitemap():
-        return sitemap('pl')
-
-    @seo.route("/sitemap.xml", host=main_domain)
+    @seo.route("/sitemap.xml")
     def main_sitemap():
-        return sitemap('en')
+        if domain_to_lang := config["DOMAIN_TO_LANG"]:
+            return sitemap(domain_to_lang[request.host])
+        else:
+            return sitemap(
+                config.get("TRANSLATION_DIRECTORIES")
+            )  # TODO should be based on localization not on config
 
     def sitemap(lang):
         """
         Route to dynamically generate a sitemap of your website/application.
         lastmod and priority tags omitted on static pages.
         lastmod included on dynamic content such as seo posts.
         """
 
         global url
         host_components = urllib.parse.urlparse(request.host_url)
         host_base = host_components.scheme + "://" + host_components.netloc
 
         # Static routes with static content
         static_urls = list()
-        for rule in seo.url_map.iter_rules():
+        for rule in current_app.url_map.iter_rules():
             if not str(rule).startswith("/admin") and not str(rule).startswith("/user"):
-                if "GET" in rule.methods and len(rule.arguments) == 0:
-                    url = {
-                        "loc": f"{host_base}{str(rule)}"
-                    }
-                static_urls.append(url)
+                if (
+                    rule.methods is not None
+                    and "GET" in rule.methods
+                    and len(rule.arguments) == 0
+                ):
+                    url = {"loc": f"{host_base}{str(rule)}"}
+                    static_urls.append(url)
 
         # Dynamic routes with dynamic content
         dynamic_urls = list()
         seo_posts = db.get_all_posts(lang)
         for post in seo_posts:
-            slug = post['slug']
-            datet = post['date'].split('T')[0]
-            url = {
-                "loc": f"{host_base}/seo/{slug}",
-                "lastmod": datet
-            }
+            slug = post["slug"]
+            datet = post["date"].split("T")[0]
+            url = {"loc": f"{host_base}/{slug}", "lastmod": datet}
             dynamic_urls.append(url)
 
-        statics = list({v['loc']: v for v in static_urls}.values())
-        dynamics = list({v['loc']: v for v in dynamic_urls}.values())
-        xml_sitemap = render_template("sitemap.xml", static_urls=statics, dynamic_urls=dynamics,
-                                      host_base=host_base)
+        statics = list({v["loc"]: v for v in static_urls}.values())
+        dynamics = list({v["loc"]: v for v in dynamic_urls}.values())
+        xml_sitemap = render_template(
+            "sitemap.xml",
+            static_urls=statics,
+            dynamic_urls=dynamics,
+            host_base=host_base,
+        )
         response = make_response(xml_sitemap)
         response.headers["Content-Type"] = "application/xml"
         return response
 
     return seo
```

### Comparing `platzky-0.1.9/platzky/static/blog.css` & `platzky-0.2.0/platzky/static/blog.css`

 * *Files 2% similar despite different names*

```diff
@@ -77,37 +77,30 @@
 }
 
 img::-moz-selection {
     color: #fff;
     background: transparent;
 }
 
-#mainNav {
-#    position: absolute;
-#    border-bottom: 1px solid #e9ecef;
-#    background-color: white;
-    font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
-}
-
 #mainNav .navbar-brand {
-    font-weight: 800;
+    font-weight: 1000;
     color: #343a40;
 }
 
 #mainNav .navbar-toggler {
-    font-size: 12px;
+    font-size: 20px;
     font-weight: 800;
-    padding: 13px;
+    padding: 10px;
     text-transform: uppercase;
     color: #343a40;
 }
 
 #mainNav .navbar-nav > li.nav-item > a {
-    font-size: 12px;
-    font-weight: 800;
+    font-size: 15px;
+    font-weight: 1000;
     letter-spacing: 1px;
     text-transform: uppercase;
 }
 
 @media only screen and (min-width: 992px) {
     #mainNav {
 	border-bottom: 1px solid transparent;
@@ -166,15 +159,15 @@
 header.masthead {
     margin-bottom: 50px;
     background: no-repeat center center;
     background-color: #868e96;
     background-attachment: scroll;
     position: relative;
     background-size: cover;
-    z-index: -1;    
+    z-index: -1;
 }
 
 header.masthead .overlay {
     position: absolute;
     top: 0;
     left: 0;
     height: 100%;
@@ -403,8 +396,8 @@
     font-size: 16px;
     padding: 25px 35px;
 }
 
 .post-content img
 {
     max-width: 100%;
-}
+}
```

### Comparing `platzky-0.1.9/platzky/templates/blog.html` & `platzky-0.2.0/platzky/templates/blog.html`

 * *Files 16% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 {{ _("Find out our tips and tricks about email marketing. We prepared some soft and some hard skills here. Ready to dive in?") }}
 {% else %}
 {{ _("You're interested in") }} {{ subtitle }}? {{ _("We're here to serve you:") }}
 {% endif %}
 {% endblock %}
 
 {% block content %}
-<div class="container">
+<div class="blog-contents mx-auto w-75">
   <h1>{% block title %}Blog {{ subtitle|default('', true) }} {% endblock %}</h1>
   {% for post in posts %}
+
   <div class="row align-items-center">
     <div class="col-3">
-      <img src={{ post.coverImage.url }} class="img-thumbnail align-middle">
+      <img src="{{ post.coverImage.url }}" alt="{{ post.coverImage.alternateText }}" class="img-thumbnail align-middle">
     </div>
     <div class="col-8 mx-auto">
       <div class="post-preview">
         <a href="{{ url_for('blog.get_post', post_slug=post.slug) }}">
           <h2 class="post-title">
             {{ post.title }}
           </h2>
```

#### html2text {}

```diff
@@ -2,14 +2,14 @@
 ("Find out our tips and tricks about email marketing. We prepared some soft and
 some hard skills here. Ready to dive in?") }} {% else %} {{ _("You're
 interested in") }} {{ subtitle }}? {{ _("We're here to serve you:") }} {% endif
 %} {% endblock %} {% block content %}
 ************ {{%% bblloocckk ttiittllee %%}}BBlloogg {{{{ ssuubbttiittllee||ddeeffaauulltt(('''',, ttrruuee)) }}}} {{%% eennddbblloocckk %%}}
 ************
 {% for post in posts %}
-[{{]
+[{{ post.coverImage.alternateText }}]
 _**_**_**_**_**_ _{{_{{_ _pp_oo_ss_tt_.._tt_ii_tt_ll_ee_ _}}_}}_ _**_**_**_**_**
 _**_**_**_**_ _{{_{{_ _pp_oo_ss_tt_.._ee_xx_cc_ee_rr_pp_tt_ _}}_}}_ _**_**_**_**
 {{ post.date }} {% for tag in post.tags %} _{_{_ _t_a_g_ _}_} {% endfor %}
 ===============================================================================
 {% endfor %}
 {% endblock %}
```

### Comparing `platzky-0.1.9/platzky/templates/feed.xml` & `platzky-0.2.0/platzky/templates/feed.xml`

 * *Files 17% similar despite different names*

#### Comparing `platzky-0.1.9/platzky/templates/feed.xml` & `platzky-0.2.0/platzky/templates/feed.xml`

```diff
@@ -1,19 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
 <rss version="2.0">
   <channel>
-    <title>{{_(&quot;Which mailing?&quot;)}}</title>
-    <link>{{ url_for(&quot;index&quot;, _external=True) }}</link>
+    <title>{{_(app_name)}}</title>
+    <link>{{ url_for(&quot;blog.all_posts&quot;, _external=True) }}</link>
     <description>{{_(&quot;Everything about mailings and newsletters&quot;)}}</description>
     {% for post in posts %}
     <item>
       <title>{{ post.title }}</title>
-      <link>{{ url_for(&quot;get_post&quot;, post_slug=post.slug, _external=True) }}</link>
+      <link>{{ url_for(&quot;blog.get_post&quot;, post_slug=post.slug, _external=True) }}</link>
       <description>{{ post.excerpt }}</description>
       <enclosure url="{{ post.coverImage.url }}" type="image/jpeg"/>
-      <guid isPermaLink="false">{{ url_for(&quot;get_post&quot;, post_slug=post.slug, _external=True) }}</guid>
+      <guid isPermaLink="false">{{ url_for(&quot;blog.get_post&quot;, post_slug=post.slug, _external=True) }}</guid>
       <pubDate>{{ post.createdAt }}</pubDate>
-      <source url="{{ url_for('get_post', post_slug=post.slug, _external=True) }}">{{_(&quot;Which mailing&quot;)}} feed</source>
+      <source url="{{ url_for('blog.get_post', post_slug=post.slug, _external=True) }}">{{_(app_name)}} feed</source>
     </item>
     {% endfor %}
   </channel>
 </rss>
```

### Comparing `platzky-0.1.9/platzky/templates/head_meta.html` & `platzky-0.2.0/platzky/templates/head_meta.html`

 * *Files 24% similar despite different names*

```diff
@@ -3,36 +3,26 @@
 <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
 <link rel="alternate" hreflang="{{language}}" href="{{ request.base_url }}"/>
 <link rel="shortcut icon" href="{{ url_for('static', filename='favicon.png') }}" type="image/x-icon">
 
 <link rel="canonical" href="{{ request.base_url }}"/>
 
 <!-- Bootstrap CSS -->
-<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet"
-      integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
+<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65" crossorigin="anonymous">
 
-<!-- MDB -->
-<link href="https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/3.1.0/mdb.min.css" rel="stylesheet">
-<!-- End MDB -->
+<!-- Flag icons -->
+<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/lipis/flag-icons@6.6.6/css/flag-icons.min.css"/>
+<!-- End Flag icons -->
 
 <!-- Font Awesome -->
 <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/css/all.min.css" rel="stylesheet">
 <!-- End Font Awesome -->
 
-
 <!-- Custom fonts for this template -->
 <link href='https://fonts.googleapis.com/css?family=Lora:400,700,400italic,700italic' rel='stylesheet' type='text/css'>
 <link
     href='https://fonts.googleapis.com/css?family=Open+Sans:300italic,400italic,600italic,700italic,800italic,400,300,600,700,800'
     rel='stylesheet' type='text/css'>
 
-<!-- Google Tag Manager -->
-<script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
-					      new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
-		     j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
-		     'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
-		    })(window,document,'script','dataLayer','GTM-MRQ7FDB');
-</script>
-<!-- End Google Tag Manager -->
-
+{{ dynamic_head | safe }}
 
 <link rel="stylesheet" type="text/css" href="{{ url_for('static', filename='blog.css') }}">
```

### Comparing `platzky-0.1.9/platzky/templates/home.html` & `platzky-0.2.0/platzky/templates/home.html`

 * *Files identical despite different names*

### Comparing `platzky-0.1.9/platzky/templates/page.html` & `platzky-0.2.0/platzky/templates/page.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 {% extends "base.html" %}
 
 {% block content %}
-<header class="masthead" style="background-image: url({{post.coverImage.url}})">
+<header class="masthead" style="background-image: url({{cover_image}})">
   <div class="overlay"></div>
   <div class="container">
     <div class="row">
       <div class="col-lg-8 col-md-10 mx-auto">
         <div class="post-heading position-relative">
-          <h1>{% block title %}{{ post.title }}{% endblock %}</h1>
+          <h1>{% block title %}{{ page.title }}{% endblock %}</h1>
         </div>
       </div>
     </div>
   </div>
 </header>
 
 <article>
   <div class="container">
     <div class="row">
       <div class="col-lg-8 col-md-10 mx-auto post-content">
-        {{post.contentInMarkdown | markdown}}
+        {{page.contentInMarkdown | markdown}}
       </div>
     </div>
   </div>
 </article>
 {% endblock %}
```

### Comparing `platzky-0.1.9/platzky/templates/post.html` & `platzky-0.2.0/platzky/templates/post.html`

 * *Files identical despite different names*

### Comparing `platzky-0.1.9/platzky/templates/sitemap.xml` & `platzky-0.2.0/platzky/templates/sitemap.xml`

 * *Files identical despite different names*

### Comparing `platzky-0.1.9/platzky/www_handler.py` & `platzky-0.2.0/platzky/www_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import urllib.parse
-from flask import request, redirect
+
+from flask import redirect, request
 
 
 def redirect_nonwww_to_www():
     """Redirect non-www requests to www."""
     urlparts = urllib.parse.urlparse(request.url)
     if not urlparts.netloc.startswith("www."):
-        urlparts = urlparts._replace(netloc=f'www.{urlparts.netloc}')
-        return redirect(urllib.parse.urlunparse(urlparts), code=301)
+        urlparts = urlparts._replace(netloc=f"www.{urlparts.netloc}")
+        url = urllib.parse.urlunparse(urlparts)
+        return redirect(url, code=301)
 
 
 def redirect_www_to_nonwww():
     """Redirect www requests to non-www."""
     urlparts = urllib.parse.urlparse(request.url)
     if urlparts.netloc.startswith("www."):
         urlparts = urlparts._replace(netloc=urlparts.netloc.removeprefix("www."))
-        return redirect(urllib.parse.urlunparse(urlparts), code=301)
+        url = urllib.parse.urlunparse(urlparts)
+        return redirect(url, code=302)
```

