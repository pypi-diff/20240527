# Comparing `tmp/banduppy-0.3.0.tar.gz` & `tmp/banduppy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banduppy-0.3.0.tar", last modified: Mon May 27 14:09:52 2024, max compression
+gzip compressed data, was "banduppy-0.3.1.tar", last modified: Mon May 27 14:36:02 2024, max compression
```

## Comparing `banduppy-0.3.0.tar` & `banduppy-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 stepan    (1000) stepan    (1000)        0 2024-05-27 14:09:52.339556 banduppy-0.3.0/
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)    35821 2024-05-27 12:47:35.000000 banduppy-0.3.0/LICENSE
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)    19435 2024-05-27 14:09:52.276398 banduppy-0.3.0/PKG-INFO
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)    19174 2024-05-27 12:47:35.000000 banduppy-0.3.0/README.md
-drwxrwxrwx   0 stepan    (1000) stepan    (1000)        0 2024-05-27 14:09:51.500118 banduppy-0.3.0/banduppy/
-drwxrwxrwx   0 stepan    (1000) stepan    (1000)        0 2024-05-27 14:09:52.091901 banduppy-0.3.0/banduppy/BasicFunctions/
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)      124 2024-05-27 12:47:35.000000 banduppy-0.3.0/banduppy/BasicFunctions/__init__.py
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)     7214 2024-05-27 12:47:35.000000 banduppy-0.3.0/banduppy/BasicFunctions/general_functions.py
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)     1313 2024-05-27 12:47:35.000000 banduppy-0.3.0/banduppy/BasicFunctions/general_plot_functions.py
-drwxrwxrwx   0 stepan    (1000) stepan    (1000)        0 2024-05-27 14:09:52.165346 banduppy-0.3.0/banduppy/Utilities/
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)    21153 2024-05-27 12:47:35.000000 banduppy-0.3.0/banduppy/Utilities/EBS_plot.py
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)    26596 2024-05-27 12:47:35.000000 banduppy-0.3.0/banduppy/Utilities/EBS_properties.py
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)      286 2024-05-27 12:47:35.000000 banduppy-0.3.0/banduppy/Utilities/__init__.py
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)     2003 2024-05-27 12:47:35.000000 banduppy-0.3.0/banduppy/Utilities/folding_degree_plot.py
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)      431 2024-05-27 14:07:02.000000 banduppy-0.3.0/banduppy/__init__.py
-drwxrwxrwx   0 stepan    (1000) stepan    (1000)        0 2024-05-27 14:09:52.224000 banduppy-0.3.0/banduppy/src/
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)      287 2024-05-27 14:04:13.000000 banduppy-0.3.0/banduppy/src/__init__.py
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)    33344 2024-05-27 14:06:05.000000 banduppy-0.3.0/banduppy/src/folding.py
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)     4523 2024-05-27 12:47:35.000000 banduppy-0.3.0/banduppy/src/folding_properties.py
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)    16923 2024-05-27 12:47:35.000000 banduppy-0.3.0/banduppy/src/unfolding.py
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)    30016 2024-05-27 12:47:35.000000 banduppy-0.3.0/banduppy/unfolding.py
-drwxrwxrwx   0 stepan    (1000) stepan    (1000)        0 2024-05-27 14:09:52.241263 banduppy-0.3.0/banduppy.egg-info/
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)    19435 2024-05-27 14:09:51.000000 banduppy-0.3.0/banduppy.egg-info/PKG-INFO
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)      620 2024-05-27 14:09:51.000000 banduppy-0.3.0/banduppy.egg-info/SOURCES.txt
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)        1 2024-05-27 14:09:51.000000 banduppy-0.3.0/banduppy.egg-info/dependency_links.txt
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)       41 2024-05-27 14:09:51.000000 banduppy-0.3.0/banduppy.egg-info/requires.txt
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)        9 2024-05-27 14:09:51.000000 banduppy-0.3.0/banduppy.egg-info/top_level.txt
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)       87 2024-05-27 14:09:52.418345 banduppy-0.3.0/setup.cfg
--rwxrwxrwx   0 stepan    (1000) stepan    (1000)      935 2024-05-27 14:04:25.000000 banduppy-0.3.0/setup.py
+drwxr-xr-x   0 stepan    (1000) stepan    (1000)        0 2024-05-27 14:36:02.779989 banduppy-0.3.1/
+-rw-r--r--   0 stepan    (1000) stepan    (1000)    35147 2024-05-27 14:21:36.000000 banduppy-0.3.1/LICENSE
+-rw-r--r--   0 stepan    (1000) stepan    (1000)    19435 2024-05-27 14:36:02.779989 banduppy-0.3.1/PKG-INFO
+-rw-r--r--   0 stepan    (1000) stepan    (1000)    18789 2024-05-27 14:21:36.000000 banduppy-0.3.1/README.md
+drwxr-xr-x   0 stepan    (1000) stepan    (1000)        0 2024-05-27 14:36:02.779989 banduppy-0.3.1/banduppy/
+drwxr-xr-x   0 stepan    (1000) stepan    (1000)        0 2024-05-27 14:36:02.779989 banduppy-0.3.1/banduppy/BasicFunctions/
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      121 2024-05-27 14:21:36.000000 banduppy-0.3.1/banduppy/BasicFunctions/__init__.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     7033 2024-05-27 14:21:36.000000 banduppy-0.3.1/banduppy/BasicFunctions/general_functions.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     1275 2024-05-27 14:21:36.000000 banduppy-0.3.1/banduppy/BasicFunctions/general_plot_functions.py
+drwxr-xr-x   0 stepan    (1000) stepan    (1000)        0 2024-05-27 14:36:02.779989 banduppy-0.3.1/banduppy/Utilities/
+-rw-r--r--   0 stepan    (1000) stepan    (1000)    20676 2024-05-27 14:21:36.000000 banduppy-0.3.1/banduppy/Utilities/EBS_plot.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)    26027 2024-05-27 14:21:36.000000 banduppy-0.3.1/banduppy/Utilities/EBS_properties.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      280 2024-05-27 14:21:36.000000 banduppy-0.3.1/banduppy/Utilities/__init__.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     1954 2024-05-27 14:21:36.000000 banduppy-0.3.1/banduppy/Utilities/folding_degree_plot.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      423 2024-05-27 14:28:05.000000 banduppy-0.3.1/banduppy/__init__.py
+drwxr-xr-x   0 stepan    (1000) stepan    (1000)        0 2024-05-27 14:36:02.779989 banduppy-0.3.1/banduppy/src/
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      258 2024-05-27 14:27:07.000000 banduppy-0.3.1/banduppy/src/__init__.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)    32623 2024-05-27 14:21:36.000000 banduppy-0.3.1/banduppy/src/folding.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     4402 2024-05-27 14:21:36.000000 banduppy-0.3.1/banduppy/src/folding_properties.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)    16528 2024-05-27 14:28:56.000000 banduppy-0.3.1/banduppy/src/unfolding.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)    29431 2024-05-27 14:21:36.000000 banduppy-0.3.1/banduppy/unfolding.py
+drwxr-xr-x   0 stepan    (1000) stepan    (1000)        0 2024-05-27 14:36:02.779989 banduppy-0.3.1/banduppy.egg-info/
+-rw-r--r--   0 stepan    (1000) stepan    (1000)    19435 2024-05-27 14:36:02.000000 banduppy-0.3.1/banduppy.egg-info/PKG-INFO
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      620 2024-05-27 14:36:02.000000 banduppy-0.3.1/banduppy.egg-info/SOURCES.txt
+-rw-r--r--   0 stepan    (1000) stepan    (1000)        1 2024-05-27 14:36:02.000000 banduppy-0.3.1/banduppy.egg-info/dependency_links.txt
+-rw-r--r--   0 stepan    (1000) stepan    (1000)       41 2024-05-27 14:36:02.000000 banduppy-0.3.1/banduppy.egg-info/requires.txt
+-rw-r--r--   0 stepan    (1000) stepan    (1000)        9 2024-05-27 14:36:02.000000 banduppy-0.3.1/banduppy.egg-info/top_level.txt
+-rw-r--r--   0 stepan    (1000) stepan    (1000)       87 2024-05-27 14:36:02.779989 banduppy-0.3.1/setup.cfg
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      910 2024-05-27 14:21:36.000000 banduppy-0.3.1/setup.py
```

### Comparing `banduppy-0.3.0/LICENSE` & `banduppy-0.3.1/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<http://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

### Comparing `banduppy-0.3.0/PKG-INFO` & `banduppy-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banduppy
-Version: 0.3.0
+Version: 0.3.1
 Summary: BandUPpy: Python interface of the BandUP code
 Home-page: https://www.ifm.liu.se/theomod/compphys/band-unfolding/
 Author: Stepan S. Tsirkin
 Author-email: stepan.tsirkin@ehu.eus
 Maintainer: Badal Mondal
 Maintainer-email: badalmondal.chembgc@gmail.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `banduppy-0.3.0/README.md` & `banduppy-0.3.1/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,385 +1,385 @@
-# `BandUP/BandUPpy`: Band Unfolding code for Plane-wave based calculations             
-# `BandUPpy` - Python version of [BandUP](https://github.com/band-unfolding/bandup) code (not to be confused with bandupy - the interface and plotting tool of BandUP)
-
-This is a Python version to the [BandUP](https://github.com/band-unfolding/bandup) code, made in order to restore
-support for modern versions of QuantumEspresso and other codes. In order ot read the wavefunctions
-stored by ab-initio codes, the routines of [irrep](https://github.com/stepan-tsirkin/irrep) are used. 
-
-<!-- =========================================================== -->
-
-<!-- =========================================================== -->
-![](imgs/Si50Ge50.png)  |  ![](imgs/Si50Ge50_.png) |  ![](imgs/SiGeOverlayBandStructure.png) |  ![](imgs/band_center_width.png)
-:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
-Unfolded band structure - flatband mode (Si0.5Ge0.5) |  Unfolded band structure - density mode (Si0.5Ge0.5) | Band structures overlay (Si0.5Ge0.5: Red, pure Si: black, pure Ge: blue) | Band centers and band width (Si0.5Ge0.5)
-<!-- =========================================================== -->
-
-<!-- =========================================================== -->
-## Developers and contributors
-<!-- =========================================================== -->
-
-__Developer of BandUPpy :__ 
-
-* [Stepan S. Tsirkin](https://github.com/stepan-tsirkin), University of Zurich, [stepan.tsirkin@uzh.ch](mailto:stepan.tsirkin@uzh.ch)
-
-__BandUPpy Package is Restructured by (maintainer):__
-
-* [Badal Mondal](https://github.com/bmondal94) 
-
-__Developer of original BandUP :__ 
-
-  *  Paulo V. C. Medeiros, Linköping University, (at present: SMHI, the Swedish Meteorological and Hydrological Institute)
-
-  *  Jonas Björk, Linköping University
-  
-  *  [Stepan S. Tsirkin](https://github.com/stepan-tsirkin), (in 2015: Donostia International Physics Center)
-
-__BandUPpy Contributors:__  [Contributors](https://github.com/band-unfolding/banduppy/graphs/contributors)
-
-* We sincerely thank each and every contributor for their valuable input and support.
-
-__Contact us:__ [Email developer/maintainer team](mailto:stepan.tsirkin@uzh.ch,badalmondal.chembgc@gmail.com) 
-
-* If you would like to contribute to the development of `BandUPpy` or request new functionality, please get in touch with [us](mailto:stepan.tsirkin@uzh.ch,badalmondal.chembgc@gmail.com) or open a pull request. We will be happy to support your request ASAP. 
-
-<!-- =========================================================== -->
-
-<!-- =========================================================== -->
-## Installation
-
-### 1. Requirements
-```
-    1. python>=3.7
-    2. collections
-    3. numpy
-    4. pickle
-    5. scipy>=1.0
-    6. irrep>=1.6.2
-    7. matplotlib
-```
-
-### 2. Installation using `pip`
-
-```
-    pip install banduppy
-```
-
-### 3. Installation from github repository
-
-```
-    git clone https://github.com/band-unfolding/banduppy.git
-    cd banduppy
-    pip install .  
-```
-
-### 4. Installation using `setup.py` [deprecated]
-Alternatively you can clone the repository and run `setup.py` in the usual manner:
-
-```
-    git clone https://github.com/band-unfolding/banduppy.git
-    cd banduppy
-    python setup.py install
-```
-<!-- =========================================================== -->
-
-<!-- =========================================================== -->
-##  Plane-wave codes currently supported by `BandUPpy`
-
-At the moment, `BandUPpy` can parse wavefunctions generated by: 
-
-  * [VASP](http://www.vasp.at)
-  * [Quantum ESPRESSO](http://www.quantum-espresso.org)
-  * [ABINIT](http://www.abinit.org)
-  * any code that has interface to [Wannier90](http://wannier.org) (via reading the UNK* and *.eig files)
-  * [CASTEP](http://www.castep.org)  --> __Not supported yet. Use the main code of BandUP.__
-
-<!-- =========================================================== -->
-
-<!-- =========================================================== -->
-## Usage
-
-Explore the [tutorial](tutorials) folder for detailed examples. Below are quick snippets showcasing what you can achieve with `BandUPpy`:
-```
-banduppy package:
-    1. Unfolding class 
-        1.1 propose_maximum_minimum_folding()
-        1.2 generate_SC_Kpts_from_pc_kpts()
-        1.3 generate_SC_Kpts_from_pc_k_path()
-        1.3 Unfold()
-        1.4 plot_ebs() [Note: Similar in Plotting class but can not plot band centers]
-    2. BandStructure class
-        2.1 BandStructure()
-    3. Properties class
-        3.1 band_centers_broadening_bandstr()
-    4. Plotting class
-        4.1 plot_ebs()
-```
-
-#### 1. Lat's start
-##### ---------------------------- Import modules ---------------------------------
-```
-    import numpy as np
-    import pickle
-    import banduppy
-```
-##### ------------------------ Define variables ---------------------------------
-###### Note: Only the VASP KPOINTS file format is implemented so far.
-```
-    # supercell : 4X4X2 supercell == np.diag([4,4,2]) or
-    super_cell_size = [[-1,  1, 1], [1, -1, 1], [1,  1, -1]] 
-    # k-path: L-G-X-U,K-G. If the segmant is skipped, put a None between nodes.
-    PC_BZ_path = [[1/2,1/2,1/2], [0,0,0],[1/2,0,1/2], [5/8,1/4,5/8], None, [3/8,3/8,3/4], [0,0,0]] 
-    # Number of k-points in each path segments. or, one single number if they are same.
-    npoints_per_path_seg = (23,27,9,29) 
-    # Labels of special k-points: list or string. e.g ['L','G','X','U','K','G'] or 'LGXUKG'
-    special_k_points = "LGXUKG"
-    # Weights of the k-points to be appended in the final generated k-points files
-    kpts_weights = 1 
-    # Save the SC kpoints in a file
-    save_to_file = True 
-    # Directory to save file
-    save_to_dir = '<directory to save files>' 
-    # File format of kpoints file that will be created and saved
-    kpts_file_format = 'vasp' # This will generate vasp KPOINTS file format
-```
-#### 1. Estimate the best choice of number of kpoints to use in effective band structure each k-path segments considering maximizing or minimizing folding in the supercell.
-##### __Motivation:__ Maximizing folding helps minimizing computational resource. 
-__Definition:__ $\text{Folding percent} = \frac{\text{no. of unique PC kpoints} \ -\ \text{no. of folded SC Kpoints}}{\text{no. of unique PC kpoints}}\times100$
-##### ------------------ Initiate Unfolding method -----------------------------
-```
-    band_unfold = banduppy.Unfolding(supercell=super_cell_size,
-                                     print_log='high')
-```
-##### ------------- Propose degree of unfolding --------------------------------
-```
-    propose_folding_results = \
-    band_unfold.propose_maximum_minimum_folding(PC_BZ_path, min_num_pts=10, max_num_pts=50,
-                                                serach_mode='brute_force', draw_plots=True, 
-                                                save_plot=False, save_dir='.', 
-                                                save_file_name=None)
-```
-#### 2. Create SC kpoints from PC band path
-##### ------------ Creating SC folded kpoints from PC band path -----------------
-__Note:__ band_unfold.generate_SC_Kpts_from_pc_kpts() can be used to generate SC Kpoints from PC kpoints list.
-```
-    kpointsPBZ_full, kpointsPBZ_unique, kpointsSBZ, \
-        SBZ_PBZ_kpts_mapping, special_kpoints_pos_labels \
-        = band_unfold.generate_SC_Kpts_from_pc_k_path(pathPBZ = PC_BZ_path,
-                                                      nk = npoints_per_path_seg,
-                                                      labels = special_k_points,
-                                                      kpts_weights = kpts_weights,
-                                                      save_all_kpts = save_to_file,
-                                                      save_sc_kpts = save_to_file,
-                                                      save_dir = save_to_dir,
-                                                      file_name_suffix = '',
-                                                      file_format=kpts_file_format)
-```
-#### 3. Unfold band structure
-```
-    read_dir = '<path where the vasp output files are>'
-```
-##### ------------------------ Read wave function file --------------------------
-```
-    bands = banduppy.BandStructure(code="vasp", spinor=False,
-                                   fPOS = f"{read_dir}/POSCAR",
-                                   fWAV = f"{read_dir}/WAVECAR")
-```
-##### ----------------- Unfold the band structures ------------------------------
-```
-    # save2file : Save unfolded kpoints or not? 
-    # fdir : Directory path where to save the file.
-    # fname : Name of the file.
-    # fname_suffix : Suffix to add to the file name.
-```
-__Option 1:__ Continue with previous instance.
-```
-    unfolded_bandstructure_, kpline \
-    = band_unfold.Unfold(bands, kline_discontinuity_threshold = 0.1, 
-                        save_unfolded_kpts = {'save2file': True, 
-                                              'fdir': save_to_dir,
-                                              'fname': 'kpoints_unfolded',
-                                              'fname_suffix': ''},
-                        save_unfolded_bandstr = {'save2file': True, 
-                                                'fdir': save_to_dir,
-                                                'fname': 'bandstructure_unfolded',
-                                                'fname_suffix': ''})
-```
-__Option 2:__ If this part is used independently from the above instances re-initiate the Unfolding module.
-```
-    # --------------------- Initiate Unfolding method --------------------------
-    band_unfold = banduppy.Unfolding(supercell=super_cell_size, print_info='high')
-
-    # ----------------- Unfold the band structures ------------------------------
-    unfolded_bandstructure_, kpline \
-    = band_unfold.Unfold(bands, PBZ_kpts_list_full=kpointsPBZ_full, 
-                         SBZ_kpts_list=kpointsSBZ, 
-                         SBZ_PBZ_kpts_map=SBZ_PBZ_kpts_mapping,
-                         kline_discontinuity_threshold = 0.1, 
-                         save_unfolded_kpts = {'save2file': True, 
-                                              'fdir': save_to_dir,
-                                              'fname': 'kpoints_unfolded',
-                                              'fname_suffix': ''},
-                         save_unfolded_bandstr = {'save2file': True, 
-                                                'fdir': save_to_dir,
-                                                'fname': 'bandstructure_unfolded',
-                                                'fname_suffix': ''})
-```
-#### 5. Determine band centers and band width
-```
-# This uses SCF algorithm of automatic band center determination from 
-# PRB 89, 041407(R) (2014) paper.
-# -------------------- Initiate Properties method -----------------------------
-    unfolded_band_properties = banduppy.Properties(print_log='high')
-    min_sum_dNs_for_a_band = 0.05 
-    threshold_dN_2b_trial_band_center = 0.05
-    prec_pos_band_centers = 1e-5 # in eV
-    err_tolerance = 1e-8
-    min_dN = 1e-5  
-    
-    unfolded_bandstructure_properties, all_scf_data = \
-        unfolded_band_properties.band_centers_broadening_bandstr(unfolded_bandstructure_, 
-                                                                 min_dN_pre_screening=min_dN,
-                                                                 threshold_dN_2b_trial_band_center=
-                                                                 threshold_dN_2b_trial_band_center,
-                                                                 min_sum_dNs_for_a_band=min_sum_dNs_for_a_band, 
-                                                                 precision_pos_band_centers=prec_pos_band_centers,
-                                                                 err_tolerance_compare_kpts=err_tolerance,
-                                                                 collect_scf_data=False)
-```
-#### 4. Plot unfolded band structure (scatter plot/density plot/band_centers plot)
-##### --------------------- Plot band structure ---------------------------------
-```
-    # Fermi energy
-    Efermi = 5.9740
-    # Minima in Energy axis to plot
-    Emin = -5
-    # Maxima in Energy axis to plot
-    Emax = 5
-    # Filename to save the figure. If None, figure will not be saved
-    save_file_name = 'unfolded_bandstructure.png'
-```
-__Option 1:__ Continue with previous instance.
-```
-    fig, ax, CountFig \
-    = band_unfold.plot_ebs(save_figure_dir=save_to_dir, save_file_name=save_file_name, CountFig=None, 
-                          Ef=Efermi, Emin=Emin, Emax=Emax, pad_energy_scale=0.5, 
-                          mode="density", special_kpoints=special_kpoints_pos_labels, 
-                          plotSC=True, fatfactor=20, nE=100,smear=0.2, marker='o',
-                          threshold_weight=0.01, show_legend=True,
-                          color='gray', color_map='viridis')
-```
-__Option 2:__ Using BandUPpy Plotting module.
-```
-    # --------------------- Initiate Plotting method ----------------------------
-    plot_unfold = banduppy.Plotting(save_figure_dir=save_to_dir)
-    
-    # -------- Read the saved unfolded bandstructure saved data file ------------
-    unfolded_bandstructure_ = np.loadtxt(f'{save_to_dir}/bandstructure_unfolded.dat')
-    kpline = np.loadtxt(f'{save_to_dir}/kpoints_unfolded.dat')[:,1]
-    with open(f'{save_to_dir}/KPOINTS_SpecialKpoints.pkl', 'rb') as handle:
-        special_kpoints_pos_labels = pickle.load(handle)
-        
-    fig, ax, CountFig \
-    = plot_unfold.plot_ebs(kpath_in_angs=kpline, unfolded_bandstructure=unfolded_bandstructure_, 
-                           save_file_name=save_file_name, CountFig=None, 
-                           Ef=Efermi, Emin=Emin, Emax=Emax, pad_energy_scale=0.5, 
-                           mode="density", special_kpoints=special_kpoints_pos_labels, 
-                           plotSC=True, fatfactor=20, nE=100,smear=0.2, marker='o',
-                           threshold_weight=0.01, show_legend=True, 
-                           color='gray', color_map='viridis')
-```
-##### ----------------- Plot the band centers -----------------------------------
-```
-    # --------------------- Initiate Plotting method ----------------------------
-    plot_unfold = banduppy.Plotting(save_figure_dir=save_to_dir)
-
-    # --------------------- Plot band centers and band width --------------------
-    fig, ax, CountFig \
-        = plot_unfold.plot_ebs(kpath_in_angs=kpline, 
-                               unfolded_bandstructure=unfolded_bandstructure_properties, 
-                               save_file_name=save_file_name, CountFig=None, 
-                               Ef=Efermi, Emin=Emin, Emax=Emax, pad_energy_scale=0.5, 
-                               mode="band_centers", special_kpoints=special_kpoints_pos_labels, 
-                               marker='x', smear=0.2, plot_colormap_bandcenter=True,
-                               color='black', color_map='viridis')
-```
-
-##### ------------ Plot and overlay multiple band structures --------------------
-```
-    fig, ax, CountFig \
-    = plot_unfold.plot_ebs(kpath_in_angs=kpline1, 
-                            unfolded_bandstructure=unfolded_bandstructure_1, 
-                            save_file_name=None, CountFig=None, threshold_weight=0.1,
-                            Ef=Efermi, Emin=Emin, Emax=Emax, pad_energy_scale=0.5, 
-                            mode="fatband", special_kpoints=special_kpoints_pos_labels1, 
-                            plotSC=True, fatfactor=20, nE=100, smear=0.2,
-                            color='red', color_map='viridis')
-    
-    fig, ax, CountFig \
-    = plot_unfold.plot_ebs(ax=ax, kpath_in_angs=kpline1, 
-                            unfolded_bandstructure=unfolded_bandstructure_properties, 
-                            save_file_name=save_file_name, CountFig=None, 
-                            Ef=Efermi, Emin=Emin, Emax=Emax, pad_energy_scale=0.5, 
-                            mode="band_centers", special_kpoints=None, 
-                            marker='x', smear=0.2,
-                            color='black', color_map='viridis')
-```
-<!-- =========================================================== -->
-
-<!-- =========================================================== -->
-## Citations and references:
-
-If you use `BandUPpy` in your work, you should:
-
-  * **State EXPLICITLY that you've used the BandUP code** 
-    (or a modified version of it, if this is the case).
-  * **Read and cite the following papers** (and the appropriate
-    references therein):
-    
->> Paulo V. C. Medeiros, Sven Stafström, and Jonas Björk,
-   [Phys. Rev. B **89**, 041407(R) (2014)](http://dx.doi.org/10.1103/PhysRevB.89.041407)  
->> Paulo V. C. Medeiros, Stepan S. Tsirkin, Sven Stafström, and Jonas Björk,
-   [Phys. Rev. B **91**, 041116(R) (2015)](http://dx.doi.org/10.1103/PhysRevB.91.041116)
-
-
-If you use `BandUPpy`,  please also cite
-
->> Mikel Iraola, Juan L. Mañes, Barry Bradlyn, Titus Neupert, Maia G. Vergniory, Stepan S. Tsirkin 
-   "IrRep: symmetry eigenvalues and irreducible representations of ab initio band structures", [arXiv:2009.01764](https://arxiv.org/abs/2009.01764)
-
-An appropriate way of acknowledging the use of BandUP in your
-publications would be, for instance, adding a sentence like: 
-
-         "The unfolding has been performed using the BandUP code"
-
-followed by the citation to our papers.
-
-### Refer to for further details
-##### <http://www.ifm.liu.se/theomod/compphys/band-unfolding>
-##### <https://github.com/band-unfolding/bandup>
-
-<!-- =========================================================== -->
-
-<!-- =========================================================== -->
-## License
-
-`BandUPpy` is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-`BandUPpy` is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with BandUP.  If not, see <http://www.gnu.org/licenses/>.
-<!-- =========================================================== -->
-
-<!-- =========================================================== -->
-## Upcoming (TBD)
-1. Effective mass implementation
-2. Scattering potential implementation
-3. Orbital contribution projection implementation
-<!-- =========================================================== -->
-
+# `BandUP/BandUPpy`: Band Unfolding code for Plane-wave based calculations             
+# `BandUPpy` - Python version of [BandUP](https://github.com/band-unfolding/bandup) code (not to be confused with bandupy - the interface and plotting tool of BandUP)
+
+This is a Python version to the [BandUP](https://github.com/band-unfolding/bandup) code, made in order to restore
+support for modern versions of QuantumEspresso and other codes. In order ot read the wavefunctions
+stored by ab-initio codes, the routines of [irrep](https://github.com/stepan-tsirkin/irrep) are used. 
+
+<!-- =========================================================== -->
+
+<!-- =========================================================== -->
+![](imgs/Si50Ge50.png)  |  ![](imgs/Si50Ge50_.png) |  ![](imgs/SiGeOverlayBandStructure.png) |  ![](imgs/band_center_width.png)
+:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
+Unfolded band structure - flatband mode (Si0.5Ge0.5) |  Unfolded band structure - density mode (Si0.5Ge0.5) | Band structures overlay (Si0.5Ge0.5: Red, pure Si: black, pure Ge: blue) | Band centers and band width (Si0.5Ge0.5)
+<!-- =========================================================== -->
+
+<!-- =========================================================== -->
+## Developers and contributors
+<!-- =========================================================== -->
+
+__Developer of BandUPpy :__ 
+
+* [Stepan S. Tsirkin](https://github.com/stepan-tsirkin), University of Zurich, [stepan.tsirkin@uzh.ch](mailto:stepan.tsirkin@uzh.ch)
+
+__BandUPpy Package is Restructured by (maintainer):__
+
+* [Badal Mondal](https://github.com/bmondal94) 
+
+__Developer of original BandUP :__ 
+
+  *  Paulo V. C. Medeiros, Linköping University, (at present: SMHI, the Swedish Meteorological and Hydrological Institute)
+
+  *  Jonas Björk, Linköping University
+  
+  *  [Stepan S. Tsirkin](https://github.com/stepan-tsirkin), (in 2015: Donostia International Physics Center)
+
+__BandUPpy Contributors:__  [Contributors](https://github.com/band-unfolding/banduppy/graphs/contributors)
+
+* We sincerely thank each and every contributor for their valuable input and support.
+
+__Contact us:__ [Email developer/maintainer team](mailto:stepan.tsirkin@uzh.ch,badalmondal.chembgc@gmail.com) 
+
+* If you would like to contribute to the development of `BandUPpy` or request new functionality, please get in touch with [us](mailto:stepan.tsirkin@uzh.ch,badalmondal.chembgc@gmail.com) or open a pull request. We will be happy to support your request ASAP. 
+
+<!-- =========================================================== -->
+
+<!-- =========================================================== -->
+## Installation
+
+### 1. Requirements
+```
+    1. python>=3.7
+    2. collections
+    3. numpy
+    4. pickle
+    5. scipy>=1.0
+    6. irrep>=1.6.2
+    7. matplotlib
+```
+
+### 2. Installation using `pip`
+
+```
+    pip install banduppy
+```
+
+### 3. Installation from github repository
+
+```
+    git clone https://github.com/band-unfolding/banduppy.git
+    cd banduppy
+    pip install .  
+```
+
+### 4. Installation using `setup.py` [deprecated]
+Alternatively you can clone the repository and run `setup.py` in the usual manner:
+
+```
+    git clone https://github.com/band-unfolding/banduppy.git
+    cd banduppy
+    python setup.py install
+```
+<!-- =========================================================== -->
+
+<!-- =========================================================== -->
+##  Plane-wave codes currently supported by `BandUPpy`
+
+At the moment, `BandUPpy` can parse wavefunctions generated by: 
+
+  * [VASP](http://www.vasp.at)
+  * [Quantum ESPRESSO](http://www.quantum-espresso.org)
+  * [ABINIT](http://www.abinit.org)
+  * any code that has interface to [Wannier90](http://wannier.org) (via reading the UNK* and *.eig files)
+  * [CASTEP](http://www.castep.org)  --> __Not supported yet. Use the main code of BandUP.__
+
+<!-- =========================================================== -->
+
+<!-- =========================================================== -->
+## Usage
+
+Explore the [tutorial](tutorials) folder for detailed examples. Below are quick snippets showcasing what you can achieve with `BandUPpy`:
+```
+banduppy package:
+    1. Unfolding class 
+        1.1 propose_maximum_minimum_folding()
+        1.2 generate_SC_Kpts_from_pc_kpts()
+        1.3 generate_SC_Kpts_from_pc_k_path()
+        1.3 Unfold()
+        1.4 plot_ebs() [Note: Similar in Plotting class but can not plot band centers]
+    2. BandStructure class
+        2.1 BandStructure()
+    3. Properties class
+        3.1 band_centers_broadening_bandstr()
+    4. Plotting class
+        4.1 plot_ebs()
+```
+
+#### 1. Lat's start
+##### ---------------------------- Import modules ---------------------------------
+```
+    import numpy as np
+    import pickle
+    import banduppy
+```
+##### ------------------------ Define variables ---------------------------------
+###### Note: Only the VASP KPOINTS file format is implemented so far.
+```
+    # supercell : 4X4X2 supercell == np.diag([4,4,2]) or
+    super_cell_size = [[-1,  1, 1], [1, -1, 1], [1,  1, -1]] 
+    # k-path: L-G-X-U,K-G. If the segmant is skipped, put a None between nodes.
+    PC_BZ_path = [[1/2,1/2,1/2], [0,0,0],[1/2,0,1/2], [5/8,1/4,5/8], None, [3/8,3/8,3/4], [0,0,0]] 
+    # Number of k-points in each path segments. or, one single number if they are same.
+    npoints_per_path_seg = (23,27,9,29) 
+    # Labels of special k-points: list or string. e.g ['L','G','X','U','K','G'] or 'LGXUKG'
+    special_k_points = "LGXUKG"
+    # Weights of the k-points to be appended in the final generated k-points files
+    kpts_weights = 1 
+    # Save the SC kpoints in a file
+    save_to_file = True 
+    # Directory to save file
+    save_to_dir = '<directory to save files>' 
+    # File format of kpoints file that will be created and saved
+    kpts_file_format = 'vasp' # This will generate vasp KPOINTS file format
+```
+#### 1. Estimate the best choice of number of kpoints to use in effective band structure each k-path segments considering maximizing or minimizing folding in the supercell.
+##### __Motivation:__ Maximizing folding helps minimizing computational resource. 
+__Definition:__ $\text{Folding percent} = \frac{\text{no. of unique PC kpoints} \ -\ \text{no. of folded SC Kpoints}}{\text{no. of unique PC kpoints}}\times100$
+##### ------------------ Initiate Unfolding method -----------------------------
+```
+    band_unfold = banduppy.Unfolding(supercell=super_cell_size,
+                                     print_log='high')
+```
+##### ------------- Propose degree of unfolding --------------------------------
+```
+    propose_folding_results = \
+    band_unfold.propose_maximum_minimum_folding(PC_BZ_path, min_num_pts=10, max_num_pts=50,
+                                                serach_mode='brute_force', draw_plots=True, 
+                                                save_plot=False, save_dir='.', 
+                                                save_file_name=None)
+```
+#### 2. Create SC kpoints from PC band path
+##### ------------ Creating SC folded kpoints from PC band path -----------------
+__Note:__ band_unfold.generate_SC_Kpts_from_pc_kpts() can be used to generate SC Kpoints from PC kpoints list.
+```
+    kpointsPBZ_full, kpointsPBZ_unique, kpointsSBZ, \
+        SBZ_PBZ_kpts_mapping, special_kpoints_pos_labels \
+        = band_unfold.generate_SC_Kpts_from_pc_k_path(pathPBZ = PC_BZ_path,
+                                                      nk = npoints_per_path_seg,
+                                                      labels = special_k_points,
+                                                      kpts_weights = kpts_weights,
+                                                      save_all_kpts = save_to_file,
+                                                      save_sc_kpts = save_to_file,
+                                                      save_dir = save_to_dir,
+                                                      file_name_suffix = '',
+                                                      file_format=kpts_file_format)
+```
+#### 3. Unfold band structure
+```
+    read_dir = '<path where the vasp output files are>'
+```
+##### ------------------------ Read wave function file --------------------------
+```
+    bands = banduppy.BandStructure(code="vasp", spinor=False,
+                                   fPOS = f"{read_dir}/POSCAR",
+                                   fWAV = f"{read_dir}/WAVECAR")
+```
+##### ----------------- Unfold the band structures ------------------------------
+```
+    # save2file : Save unfolded kpoints or not? 
+    # fdir : Directory path where to save the file.
+    # fname : Name of the file.
+    # fname_suffix : Suffix to add to the file name.
+```
+__Option 1:__ Continue with previous instance.
+```
+    unfolded_bandstructure_, kpline \
+    = band_unfold.Unfold(bands, kline_discontinuity_threshold = 0.1, 
+                        save_unfolded_kpts = {'save2file': True, 
+                                              'fdir': save_to_dir,
+                                              'fname': 'kpoints_unfolded',
+                                              'fname_suffix': ''},
+                        save_unfolded_bandstr = {'save2file': True, 
+                                                'fdir': save_to_dir,
+                                                'fname': 'bandstructure_unfolded',
+                                                'fname_suffix': ''})
+```
+__Option 2:__ If this part is used independently from the above instances re-initiate the Unfolding module.
+```
+    # --------------------- Initiate Unfolding method --------------------------
+    band_unfold = banduppy.Unfolding(supercell=super_cell_size, print_info='high')
+
+    # ----------------- Unfold the band structures ------------------------------
+    unfolded_bandstructure_, kpline \
+    = band_unfold.Unfold(bands, PBZ_kpts_list_full=kpointsPBZ_full, 
+                         SBZ_kpts_list=kpointsSBZ, 
+                         SBZ_PBZ_kpts_map=SBZ_PBZ_kpts_mapping,
+                         kline_discontinuity_threshold = 0.1, 
+                         save_unfolded_kpts = {'save2file': True, 
+                                              'fdir': save_to_dir,
+                                              'fname': 'kpoints_unfolded',
+                                              'fname_suffix': ''},
+                         save_unfolded_bandstr = {'save2file': True, 
+                                                'fdir': save_to_dir,
+                                                'fname': 'bandstructure_unfolded',
+                                                'fname_suffix': ''})
+```
+#### 5. Determine band centers and band width
+```
+# This uses SCF algorithm of automatic band center determination from 
+# PRB 89, 041407(R) (2014) paper.
+# -------------------- Initiate Properties method -----------------------------
+    unfolded_band_properties = banduppy.Properties(print_log='high')
+    min_sum_dNs_for_a_band = 0.05 
+    threshold_dN_2b_trial_band_center = 0.05
+    prec_pos_band_centers = 1e-5 # in eV
+    err_tolerance = 1e-8
+    min_dN = 1e-5  
+    
+    unfolded_bandstructure_properties, all_scf_data = \
+        unfolded_band_properties.band_centers_broadening_bandstr(unfolded_bandstructure_, 
+                                                                 min_dN_pre_screening=min_dN,
+                                                                 threshold_dN_2b_trial_band_center=
+                                                                 threshold_dN_2b_trial_band_center,
+                                                                 min_sum_dNs_for_a_band=min_sum_dNs_for_a_band, 
+                                                                 precision_pos_band_centers=prec_pos_band_centers,
+                                                                 err_tolerance_compare_kpts=err_tolerance,
+                                                                 collect_scf_data=False)
+```
+#### 4. Plot unfolded band structure (scatter plot/density plot/band_centers plot)
+##### --------------------- Plot band structure ---------------------------------
+```
+    # Fermi energy
+    Efermi = 5.9740
+    # Minima in Energy axis to plot
+    Emin = -5
+    # Maxima in Energy axis to plot
+    Emax = 5
+    # Filename to save the figure. If None, figure will not be saved
+    save_file_name = 'unfolded_bandstructure.png'
+```
+__Option 1:__ Continue with previous instance.
+```
+    fig, ax, CountFig \
+    = band_unfold.plot_ebs(save_figure_dir=save_to_dir, save_file_name=save_file_name, CountFig=None, 
+                          Ef=Efermi, Emin=Emin, Emax=Emax, pad_energy_scale=0.5, 
+                          mode="density", special_kpoints=special_kpoints_pos_labels, 
+                          plotSC=True, fatfactor=20, nE=100,smear=0.2, marker='o',
+                          threshold_weight=0.01, show_legend=True,
+                          color='gray', color_map='viridis')
+```
+__Option 2:__ Using BandUPpy Plotting module.
+```
+    # --------------------- Initiate Plotting method ----------------------------
+    plot_unfold = banduppy.Plotting(save_figure_dir=save_to_dir)
+    
+    # -------- Read the saved unfolded bandstructure saved data file ------------
+    unfolded_bandstructure_ = np.loadtxt(f'{save_to_dir}/bandstructure_unfolded.dat')
+    kpline = np.loadtxt(f'{save_to_dir}/kpoints_unfolded.dat')[:,1]
+    with open(f'{save_to_dir}/KPOINTS_SpecialKpoints.pkl', 'rb') as handle:
+        special_kpoints_pos_labels = pickle.load(handle)
+        
+    fig, ax, CountFig \
+    = plot_unfold.plot_ebs(kpath_in_angs=kpline, unfolded_bandstructure=unfolded_bandstructure_, 
+                           save_file_name=save_file_name, CountFig=None, 
+                           Ef=Efermi, Emin=Emin, Emax=Emax, pad_energy_scale=0.5, 
+                           mode="density", special_kpoints=special_kpoints_pos_labels, 
+                           plotSC=True, fatfactor=20, nE=100,smear=0.2, marker='o',
+                           threshold_weight=0.01, show_legend=True, 
+                           color='gray', color_map='viridis')
+```
+##### ----------------- Plot the band centers -----------------------------------
+```
+    # --------------------- Initiate Plotting method ----------------------------
+    plot_unfold = banduppy.Plotting(save_figure_dir=save_to_dir)
+
+    # --------------------- Plot band centers and band width --------------------
+    fig, ax, CountFig \
+        = plot_unfold.plot_ebs(kpath_in_angs=kpline, 
+                               unfolded_bandstructure=unfolded_bandstructure_properties, 
+                               save_file_name=save_file_name, CountFig=None, 
+                               Ef=Efermi, Emin=Emin, Emax=Emax, pad_energy_scale=0.5, 
+                               mode="band_centers", special_kpoints=special_kpoints_pos_labels, 
+                               marker='x', smear=0.2, plot_colormap_bandcenter=True,
+                               color='black', color_map='viridis')
+```
+
+##### ------------ Plot and overlay multiple band structures --------------------
+```
+    fig, ax, CountFig \
+    = plot_unfold.plot_ebs(kpath_in_angs=kpline1, 
+                            unfolded_bandstructure=unfolded_bandstructure_1, 
+                            save_file_name=None, CountFig=None, threshold_weight=0.1,
+                            Ef=Efermi, Emin=Emin, Emax=Emax, pad_energy_scale=0.5, 
+                            mode="fatband", special_kpoints=special_kpoints_pos_labels1, 
+                            plotSC=True, fatfactor=20, nE=100, smear=0.2,
+                            color='red', color_map='viridis')
+    
+    fig, ax, CountFig \
+    = plot_unfold.plot_ebs(ax=ax, kpath_in_angs=kpline1, 
+                            unfolded_bandstructure=unfolded_bandstructure_properties, 
+                            save_file_name=save_file_name, CountFig=None, 
+                            Ef=Efermi, Emin=Emin, Emax=Emax, pad_energy_scale=0.5, 
+                            mode="band_centers", special_kpoints=None, 
+                            marker='x', smear=0.2,
+                            color='black', color_map='viridis')
+```
+<!-- =========================================================== -->
+
+<!-- =========================================================== -->
+## Citations and references:
+
+If you use `BandUPpy` in your work, you should:
+
+  * **State EXPLICITLY that you've used the BandUP code** 
+    (or a modified version of it, if this is the case).
+  * **Read and cite the following papers** (and the appropriate
+    references therein):
+    
+>> Paulo V. C. Medeiros, Sven Stafström, and Jonas Björk,
+   [Phys. Rev. B **89**, 041407(R) (2014)](http://dx.doi.org/10.1103/PhysRevB.89.041407)  
+>> Paulo V. C. Medeiros, Stepan S. Tsirkin, Sven Stafström, and Jonas Björk,
+   [Phys. Rev. B **91**, 041116(R) (2015)](http://dx.doi.org/10.1103/PhysRevB.91.041116)
+
+
+If you use `BandUPpy`,  please also cite
+
+>> Mikel Iraola, Juan L. Mañes, Barry Bradlyn, Titus Neupert, Maia G. Vergniory, Stepan S. Tsirkin 
+   "IrRep: symmetry eigenvalues and irreducible representations of ab initio band structures", [arXiv:2009.01764](https://arxiv.org/abs/2009.01764)
+
+An appropriate way of acknowledging the use of BandUP in your
+publications would be, for instance, adding a sentence like: 
+
+         "The unfolding has been performed using the BandUP code"
+
+followed by the citation to our papers.
+
+### Refer to for further details
+##### <http://www.ifm.liu.se/theomod/compphys/band-unfolding>
+##### <https://github.com/band-unfolding/bandup>
+
+<!-- =========================================================== -->
+
+<!-- =========================================================== -->
+## License
+
+`BandUPpy` is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+`BandUPpy` is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with BandUP.  If not, see <http://www.gnu.org/licenses/>.
+<!-- =========================================================== -->
+
+<!-- =========================================================== -->
+## Upcoming (TBD)
+1. Effective mass implementation
+2. Scattering potential implementation
+3. Orbital contribution projection implementation
+<!-- =========================================================== -->
+
```

### Comparing `banduppy-0.3.0/banduppy/BasicFunctions/general_functions.py` & `banduppy-0.3.1/banduppy/BasicFunctions/general_functions.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-import numpy as np
-import pickle
-
-_draw_line_length = 72
-
-## ============================================================================   
-class _BasicFunctionsModule(object):
-    
-    @staticmethod
-    def _check_transformation_matrix(M, tolerance = 1e-14):
-        """
-        Check shape and commensurate property of PC-SC transformation matrix.
-
-        Parameters
-        ----------
-        M : ndarray
-            Matrix to check.
-        tolerance : float, optional
-            Tolerance to check if transformation matrix is commensurate. The default is 1e-14.
-
-        Returns
-        -------
-        M_f : ndarray of int
-            Transformation matrix.
-
-        """
-        assert M.shape==(3,3), "supercell should be 3x3, found {}".format(M.shape)
-        
-        M_int = np.round(M)
-        assert np.linalg.norm(np.array(M) - M_int) < tolerance , "supercell should consist of integers, found {}".format(M)
-        
-        M_f = np.array(M_int,dtype=int)
-        assert np.linalg.det(M_f) != 0, "the supercell vectors should be linear independent"
-        
-        return M_f
-    
-    @staticmethod
-    def _round_2_tolerance(input_array, decimals=10):
-        '''
-        Use rounding to avoid flotting point precision.
-        o 0.1%1 != 1.1%1
-        o 0.1%1 == np.round(1.1%1, decimals=10)
-        '''
-        return np.round(input_array, decimals=decimals)
-    
-    @staticmethod
-    def _return_mod(input_array, round_decimals:bool=True):
-        """
-        Return mod value. => Scale k-points.
-
-        Parameters
-        ----------
-        input_array : numpy ndarray
-            Input array to round decimals.
-        round_decimals : bool, optional
-            Round decimals or not? The default is True.
-
-        Returns
-        -------
-        numpy ndarray
-            After rounding the float decimal points.
-
-        """
-        if round_decimals:
-            return _BasicFunctionsModule._round_2_tolerance(input_array%1)
-        else:
-            return input_array%1
-        
-## ============================================================================
-class SaveData2File:
-    def __init__(self):
-        pass
-    
-    @staticmethod
-    def default_save_settings(save_data):
-        tmp_save = {'save2file': False, 'fdir': '.', 'fname': 'test', 'fname_suffix': ''}
-        for ll in tmp_save:
-            if ll in save_data:
-                tmp_save[ll] = save_data[ll]
-        return tmp_save
-    
-    @staticmethod
-    def save_2_file(data=None, save_dir='.', file_name:str='', file_name_suffix:str='', 
-                    header_txt:str='', footer_txt:str='',comments_symbol='! ',
-                    np_data_fmt='%12.8f', print_log:bool=True):
-        """
-        Save the generated SC kpoints to a file.
-
-        Parameters
-        ----------
-        data : numpy array, optional
-            Data to be saved. The default is None.
-        save_dir : str/path_object, optional
-            Directory to save the file. The default is current directory.
-        file_name : str, optional
-            Name of the file. The default is ''.
-            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
-        file_name_suffix : str, optional
-            Suffix to add after the file_name. The default is ''.
-        header_txt : str, optional
-            String that will be written at the beginning of the file. The default is None.
-        footer_txt : str, optional
-            String that will be written at the end of the file.. The default is None.
-        comments_symbol : str, optional
-            String that will be prepended to the header and footer strings, 
-            to mark them as comments. The default is ‘!‘. 
-        np_data_fmt: str
-            Data format for numpy.savetxt.
-        print_log : bool, optional
-            Print path of save file. The default is False.
-
-        Returns
-        -------
-        String/path object
-            File path where the data is saved.
-
-        """
-        if data is None: return
-        fname_save_file = f'{save_dir}/{file_name}{file_name_suffix}'
-        if isinstance(data, np.ndarray):
-            with open(fname_save_file, 'w') as f:
-                np.savetxt(f, data, header=header_txt, footer=footer_txt, 
-                           fmt=np_data_fmt, comments=comments_symbol)
-        elif isinstance(data, dict):
-            fname_save_file += '.pkl'
-            with open(fname_save_file, 'wb') as f:
-                # Note: the header and footer msg are not saved for the time being.
-                pickle.dump(data, f, protocol=pickle.HIGHEST_PROTOCOL)
-        return fname_save_file
-    
-    @staticmethod
-    def save_sc_kpts_2_file(data=None, save_dir='.', file_name:str='', 
-                            file_name_suffix:str='', file_format:str='vasp',
-                            header_txt:str='', footer_txt:str='',comments_symbol='! ',
-                            print_log:bool=False, print_msg:str='Saving to file...'):
-        """
-        Save the generated SC kpoints to a file.
-
-        Parameters
-        ----------
-        data : numpy array, optional
-            Data to be saved. The default is None.
-        save_dir : str/path_object, optional
-            Directory to save the file. The default is current directory.
-        file_name : str, optional
-            Name of the file. The default is ''.
-            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
-        file_name_suffix : str, optional
-            Suffix to add after the file_name. The default is ''.
-        file_format : ['vasp'], optional
-            Format of the file. The default is 'vasp'. 
-            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
-        header_txt : str, optional
-            String that will be written at the beginning of the file. The default is None.
-        footer_txt : str, optional
-            String that will be written at the end of the file.. The default is None.
-        comments_symbol : str, optional
-            String that will be prepended to the header and footer strings, 
-            to mark them as comments. The default is ‘!‘. 
-        print_log : bool, optional
-            Print path of save file. The default is False.
-        print_msg : str, optional
-            Message to print on print_log. The default is ''.
-
-        Returns
-        -------
-        String/path object
-            File path where the data is saved.
-
-        """
-        if file_format == 'vasp':
-            file_name = 'KPOINTS'
-            comments_symbol = ''
-            
-        if print_log: print(f"{'='*_draw_line_length}\n- {print_msg}.")
-        
-        fname_save_file = \
-        SaveData2File.save_2_file(data=data, save_dir=save_dir, file_name=file_name, 
-                                  file_name_suffix=file_name_suffix, header_txt=header_txt, 
-                                  footer_txt=footer_txt,comments_symbol=comments_symbol)
-        if print_log: print(f'-- Filepath: {fname_save_file}\n- Done')
+import numpy as np
+import pickle
+
+_draw_line_length = 72
+
+## ============================================================================   
+class _BasicFunctionsModule(object):
+    
+    @staticmethod
+    def _check_transformation_matrix(M, tolerance = 1e-14):
+        """
+        Check shape and commensurate property of PC-SC transformation matrix.
+
+        Parameters
+        ----------
+        M : ndarray
+            Matrix to check.
+        tolerance : float, optional
+            Tolerance to check if transformation matrix is commensurate. The default is 1e-14.
+
+        Returns
+        -------
+        M_f : ndarray of int
+            Transformation matrix.
+
+        """
+        assert M.shape==(3,3), "supercell should be 3x3, found {}".format(M.shape)
+        
+        M_int = np.round(M)
+        assert np.linalg.norm(np.array(M) - M_int) < tolerance , "supercell should consist of integers, found {}".format(M)
+        
+        M_f = np.array(M_int,dtype=int)
+        assert np.linalg.det(M_f) != 0, "the supercell vectors should be linear independent"
+        
+        return M_f
+    
+    @staticmethod
+    def _round_2_tolerance(input_array, decimals=10):
+        '''
+        Use rounding to avoid flotting point precision.
+        o 0.1%1 != 1.1%1
+        o 0.1%1 == np.round(1.1%1, decimals=10)
+        '''
+        return np.round(input_array, decimals=decimals)
+    
+    @staticmethod
+    def _return_mod(input_array, round_decimals:bool=True):
+        """
+        Return mod value. => Scale k-points.
+
+        Parameters
+        ----------
+        input_array : numpy ndarray
+            Input array to round decimals.
+        round_decimals : bool, optional
+            Round decimals or not? The default is True.
+
+        Returns
+        -------
+        numpy ndarray
+            After rounding the float decimal points.
+
+        """
+        if round_decimals:
+            return _BasicFunctionsModule._round_2_tolerance(input_array%1)
+        else:
+            return input_array%1
+        
+## ============================================================================
+class SaveData2File:
+    def __init__(self):
+        pass
+    
+    @staticmethod
+    def default_save_settings(save_data):
+        tmp_save = {'save2file': False, 'fdir': '.', 'fname': 'test', 'fname_suffix': ''}
+        for ll in tmp_save:
+            if ll in save_data:
+                tmp_save[ll] = save_data[ll]
+        return tmp_save
+    
+    @staticmethod
+    def save_2_file(data=None, save_dir='.', file_name:str='', file_name_suffix:str='', 
+                    header_txt:str='', footer_txt:str='',comments_symbol='! ',
+                    np_data_fmt='%12.8f', print_log:bool=True):
+        """
+        Save the generated SC kpoints to a file.
+
+        Parameters
+        ----------
+        data : numpy array, optional
+            Data to be saved. The default is None.
+        save_dir : str/path_object, optional
+            Directory to save the file. The default is current directory.
+        file_name : str, optional
+            Name of the file. The default is ''.
+            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
+        file_name_suffix : str, optional
+            Suffix to add after the file_name. The default is ''.
+        header_txt : str, optional
+            String that will be written at the beginning of the file. The default is None.
+        footer_txt : str, optional
+            String that will be written at the end of the file.. The default is None.
+        comments_symbol : str, optional
+            String that will be prepended to the header and footer strings, 
+            to mark them as comments. The default is ‘!‘. 
+        np_data_fmt: str
+            Data format for numpy.savetxt.
+        print_log : bool, optional
+            Print path of save file. The default is False.
+
+        Returns
+        -------
+        String/path object
+            File path where the data is saved.
+
+        """
+        if data is None: return
+        fname_save_file = f'{save_dir}/{file_name}{file_name_suffix}'
+        if isinstance(data, np.ndarray):
+            with open(fname_save_file, 'w') as f:
+                np.savetxt(f, data, header=header_txt, footer=footer_txt, 
+                           fmt=np_data_fmt, comments=comments_symbol)
+        elif isinstance(data, dict):
+            fname_save_file += '.pkl'
+            with open(fname_save_file, 'wb') as f:
+                # Note: the header and footer msg are not saved for the time being.
+                pickle.dump(data, f, protocol=pickle.HIGHEST_PROTOCOL)
+        return fname_save_file
+    
+    @staticmethod
+    def save_sc_kpts_2_file(data=None, save_dir='.', file_name:str='', 
+                            file_name_suffix:str='', file_format:str='vasp',
+                            header_txt:str='', footer_txt:str='',comments_symbol='! ',
+                            print_log:bool=False, print_msg:str='Saving to file...'):
+        """
+        Save the generated SC kpoints to a file.
+
+        Parameters
+        ----------
+        data : numpy array, optional
+            Data to be saved. The default is None.
+        save_dir : str/path_object, optional
+            Directory to save the file. The default is current directory.
+        file_name : str, optional
+            Name of the file. The default is ''.
+            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
+        file_name_suffix : str, optional
+            Suffix to add after the file_name. The default is ''.
+        file_format : ['vasp'], optional
+            Format of the file. The default is 'vasp'. 
+            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
+        header_txt : str, optional
+            String that will be written at the beginning of the file. The default is None.
+        footer_txt : str, optional
+            String that will be written at the end of the file.. The default is None.
+        comments_symbol : str, optional
+            String that will be prepended to the header and footer strings, 
+            to mark them as comments. The default is ‘!‘. 
+        print_log : bool, optional
+            Print path of save file. The default is False.
+        print_msg : str, optional
+            Message to print on print_log. The default is ''.
+
+        Returns
+        -------
+        String/path object
+            File path where the data is saved.
+
+        """
+        if file_format == 'vasp':
+            file_name = 'KPOINTS'
+            comments_symbol = ''
+            
+        if print_log: print(f"{'='*_draw_line_length}\n- {print_msg}.")
+        
+        fname_save_file = \
+        SaveData2File.save_2_file(data=data, save_dir=save_dir, file_name=file_name, 
+                                  file_name_suffix=file_name_suffix, header_txt=header_txt, 
+                                  footer_txt=footer_txt,comments_symbol=comments_symbol)
+        if print_log: print(f'-- Filepath: {fname_save_file}\n- Done')
         return fname_save_file
```

### Comparing `banduppy-0.3.0/banduppy/Utilities/EBS_plot.py` & `banduppy-0.3.1/banduppy/Utilities/EBS_plot.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,478 +1,478 @@
-import numpy as np
-import matplotlib.pyplot as plt
-from ..BasicFunctions.general_plot_functions import GeneratePlots
-from .EBS_properties import _FormatSpecialKpts
-
-### ===========================================================================
-
-class EBSplot(GeneratePlots, _FormatSpecialKpts):
-    """
-    Plotting (effective) band structures and related.
-
-    """
-    def __init__(self, kpath_in_angs=None, unfolded_bandstructure=None,
-                 save_figure_dir='.'):
-        """
-        Initialize the band structure plotting class.
-
-        Parameters
-        ----------
-        kpath_in_angs : array, optional
-            k on path (in A^-1) coordinate. The default is None.
-        unfolded_bandstructure : ndarray, optional
-            Unfolded effective band structure data. 
-            Format: k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
-            The default is None.
-        save_figure_dir : str/path, optional
-            Directory where to save the figure. The default is current directory.
-
-        """
-        GeneratePlots.__init__(self, save_figure_dir=save_figure_dir)
-        self.efermi = 0.0
-        
-        if kpath_in_angs is None:
-            try:
-                self.kpath_in_angs_ = self.kpline.copy()
-            except:
-                raise ValueError('No bandstructure data file is found')
-        else:
-            self.kpath_in_angs_ = kpath_in_angs.copy()
-        
-        if unfolded_bandstructure is None:
-            try:
-                self.plot_result = self.unfolded_bandstructure.copy()
-            except:
-                raise ValueError('No bandstructure data file is found')
-        else:
-            self.plot_result = unfolded_bandstructure.copy()
-        
-
-    # def plot(self, ax=None, save_file_name=None, CountFig=None, Ef=None, Emin=None, 
-    #          Emax=None,  pad_energy_scale:float=0.5, threshold_weight:float=None,  
-    #          mode:str="fatband", yaxis_label:str='E (eV)', special_kpoints:dict=None, 
-    #          plotSC:bool=True, marker='o', fatfactor=20, nE:int=100, smear:float=0.05,  
-    #          scatter_color='gray', color_map='viridis', show_legend:bool=True):
-    #     """
-    #     Scatter/density plot of the band structure.
-
-    #     Parameters
-    #     ----------
-    #     ax : matplotlib.pyplot axis, optional
-    #         Figure axis to plot on. If None, new figure will be created.
-    #         The default is None.
-    #     save_file_name : str, optional
-    #         Name of the figure file. If None, figure will be not saved. 
-    #         The default is None.
-    #     CountFig: int, optional
-    #         Figure count. The default is None.
-    #     Ef : float, optional
-    #         Fermi energy. If None, set to 0.0. The default is None.
-    #     Emin : float, optional
-    #         Minimum in energy. The default is None.
-    #     Emax : float, optional
-    #         Maximum in energy. The default is None.
-    #     pad_energy_scale: float, optional
-    #         Add padding of pad_energy_scale to minimum and maximum energy if Emin
-    #         and Emax are None. The default is 0.5.
-    #     threshold_weight : float, optional
-    #         The band centers with band weights lower than the threshhold weights 
-    #         are discarded. The default is None. If None, this is ignored.
-    #     mode : ['fatband','density'], optional
-    #         Mode of plot. The default is "fatband".
-    #     yaxis_label : str, optional
-    #         Y-axis label text. The default is 'E (eV)'.
-    #     special_kpoints : dictionary, optional
-    #         Dictionary of special kpoints position and labels. If None, ignore
-    #         special kpoints. The default is None.
-    #     plotSC : bool, optional
-    #         Plot supercell bandstructure. The default is True.
-    #     marker : matplotlib.pyplot markerMarkerStyle, optional
-    #         The marker style. Marker can be either an instance of the class or 
-    #         the text shorthand for a particular marker. 
-    #         The default is 'o'.
-    #     fatfactor : int, optional
-    #         Scatter plot marker size. The default is 20.
-    #     nE : int, optional
-    #         Number of pixels in Energy scale when used 'density' mode. 
-    #         The default is 100.
-    #     smear : float, optional
-    #         Gaussian smearing. The default is 0.05.
-    #     scatter_color : str/color, optional
-    #         Color of scatter plot of unfolded band structure. The color of supercell
-    #         band structures is gray. The default is 'gray'.
-    #     color_map: str/ matplotlib colormap
-    #         Colormap for density plot. The default is viridis.
-    #     show_legend : bool
-    #         If show legend or not. The default is True.
-        
-    #     Raises
-    #     ------
-    #     ValueError
-    #         If plot mode is unknown.
-
-    #     Returns
-    #     -------
-    #     fig : matplotlib.pyplot.figure
-    #         Figure instance. If ax is not None previously generated fig instance
-    #         will be used.
-    #     ax : Axis instance
-    #         Figure axis instance.
-    #     CountFig: int or None
-    #         Figure count.
-
-    #     """
-        
-    #     print('- Plotting band structures...')
-    #     if ax is None: 
-    #         self.fig, ax = plt.subplots()
-        
-    #     if Ef == 'auto' or Ef is None: 
-    #         Ef = self.efermi
-    #     # Shift the energy scale to 0 fermi energy level   
-    #     if Ef is not None:
-    #         self.plot_result[:,2] -= Ef 
-    #         ax.axhline(y=0, color='k', ls='--', lw=1)
-    #         yaxis_label = r"E$-$E$_\mathrm{F}$ (eV)"
-    #         print(f"-- Efermi was set to {Ef} eV")
- 
-    #     if Emin is None: Emin = self.plot_result[:,2].min() - pad_energy_scale
-    #     if Emax is None: Emax = self.plot_result[:,2].max() + pad_energy_scale
-        
-    #     result_ = self.plot_result[(self.plot_result[:,2] >= Emin - max(smear*10, 0.1)) * 
-    #                                (self.plot_result[:,2] <= Emax + max(smear*10, 0.1))]
-    #     result = result_[:, 1:]
-    #     # Set weights to 0 which are below threshold_weight
-    #     if threshold_weight is not None: 
-    #         result[result[:, 2] < threshold_weight, 2] = 0
-        
-    #     # Plot as fat band
-    #     if mode == "fatband":
-    #         if plotSC:
-    #             ax.scatter(result[:, 0], result[:, 1], s=fatfactor, color='gray', label="supercell")
-    #         ax.scatter(result[:, 0], result[:, 1], s=result[:, 2]*fatfactor, 
-    #                    marker=marker, color=scatter_color, label="unfolded")
-    #         if show_legend: ax.legend(loc=1)
-    #     elif mode == "density":
-    #         energy = np.linspace(Emin, Emax, nE)
-    #         density = np.zeros((len(self.kpath_in_angs_),nE), dtype=float)
-    #         for k, E, w in result[:, :3]:
-    #             ik = np.argmin(abs(k - self.kpath_in_angs_))
-    #             # Gaussian smearing
-    #             density[ik, :] += w*np.exp(-(energy-E)**2/(2*smear**2)) 
-    #         # density=np.log(density)
-    #         # density[density<1e-3]=0           
-    #         k1 = np.hstack(([self.kpath_in_angs_[0]], 
-    #                         (self.kpath_in_angs_[1:]+self.kpath_in_angs_[:-1])/2,
-    #                         [self.kpath_in_angs_[-1]]))
-    #         E1 = np.hstack(([energy[0]],(energy[1:]+energy[:-1])/2,[energy[-1]]))
-    #         # print(k1,E1)
-    #         # density=np.pad(density,((0,1),(0,1)))
-    #         # print("before",k1.shape,E1.shape,density.shape)
-    #         k1, E1 = np.meshgrid(k1,E1)
-    #         # print("after",k1.shape,E1.shape,density.shape)
-    #         plt.pcolormesh(k1, E1, density.T, cmap=color_map)
-    #         plt.colorbar()
-    #     else:
-    #         raise ValueError("Unknownplot mode: '{}'".format(mode))
-            
-    #     if special_kpoints is not None:
-    #         x_tiks_labels, x_tiks_positions = \
-    #             _FormatSpecialKpts._extract_special_kpts_info(special_kpoints, 
-    #                                                           self.kpath_in_angs_)
-    #         plt.xticks(x_tiks_positions, x_tiks_labels)
-    #         # Draw vertical lines
-    #         for line_pos in x_tiks_positions:
-    #             plt.axvline(x=line_pos, color='k', ls='--', lw=2)
-        
-    #     ax.set_ylabel(yaxis_label)
-    #     ax.set_ylim([Emin, Emax])
-    #     ax.set_xlim([self.kpath_in_angs_.min(), self.kpath_in_angs_.max()])
-
-    #     if save_file_name is None:
-    #         plt.show()
-    #     else:
-    #         CountFig = self.save_figure(save_file_name, CountFig=CountFig)
-    #         plt.close()
-    #     return self.fig, ax, CountFig
-    
-    def plot(self, ax=None, save_file_name=None, CountFig=None, Ef=None, Emin=None, 
-             Emax=None,  pad_energy_scale:float=0.5, threshold_weight:float=None,  
-             mode:str="fatband", yaxis_label:str='E (eV)', special_kpoints:dict=None, 
-             plotSC:bool=True, marker='o', fatfactor=20, nE:int=100, smear:float=0.05,  
-             color='gray', color_map='viridis', plot_colormap_bandcenter:bool=True,
-             show_legend:bool=True):
-        """
-        Scatter/density plot of the band structure.
-
-        Parameters
-        ----------
-        ax : matplotlib.pyplot axis, optional
-            Figure axis to plot on. If None, new figure will be created.
-            The default is None.
-        save_file_name : str, optional
-            Name of the figure file. If None, figure will be not saved. 
-            The default is None.
-        CountFig: int, optional
-            Figure count. The default is None.
-        Ef : float, optional
-            Fermi energy. If None, set to 0.0. The default is None.
-        Emin : float, optional
-            Minimum in energy. The default is None.
-        Emax : float, optional
-            Maximum in energy. The default is None.
-        pad_energy_scale: float, optional
-            Add padding of pad_energy_scale to minimum and maximum energy if Emin
-            and Emax are None. The default is 0.5.
-        threshold_weight : float, optional
-            The band centers with band weights lower than the threshhold weights 
-            are discarded. The default is None. If None, this is ignored.
-        mode : ['fatband','density', 'band_centers'], optional
-            Mode of plot. The default is "fatband".
-        yaxis_label : str, optional
-            Y-axis label text. The default is 'E (eV)'.
-        special_kpoints : dictionary, optional
-            Dictionary of special kpoints position and labels. If None, ignore
-            special kpoints. The default is None.
-        plotSC : bool, optional
-            Plot supercell bandstructure. The default is True.
-        marker : matplotlib.pyplot markerMarkerStyle, optional
-            The marker style. Marker can be either an instance of the class or 
-            the text shorthand for a particular marker. 
-            The default is 'o'.
-        fatfactor : int, optional
-            Scatter plot marker size. The default is 20.
-        nE : int, optional
-            Number of pixels in Energy scale when used 'density' mode. 
-            The default is 100.
-        smear : float, optional
-            Gaussian smearing. The default is 0.05.
-        color : str/color, optional
-            Color of plot of unfolded band structure. The color of supercell
-            band structures is gray. The default is 'gray'.
-        color_map: str/ matplotlib colormap
-            Colormap for density plot. The default is viridis.
-        plot_colormap_bandcenter : bool, optional
-            If plotting the band ceneters by colormap. The default is True.
-        show_legend : bool, optional
-            If show legend or not. The default is True.
-        
-        Raises
-        ------
-        ValueError
-            If plot mode is unknown.
-
-        Returns
-        -------
-        fig : matplotlib.pyplot.figure
-            Figure instance. If ax is not None previously generated fig instance
-            will be used.
-        ax : Axis instance
-            Figure axis instance.
-        CountFig: int or None
-            Figure count.
-
-        """
-        
-        print('- Plotting band structures...')
-        if ax is None: 
-            self.fig, ax = plt.subplots()
-        
-        if mode != "band_centers" and len(self.plot_result[0]) > 3: 
-            self.plot_result = self.plot_result[:, 1:]
-        
-        if Ef == 'auto' or Ef is None: 
-            Ef = self.efermi
-        # Shift the energy scale to 0 fermi energy level   
-        if Ef is not None:
-            self.plot_result[:, 1] -= Ef 
-            ax.axhline(y=0, color='k', ls='--', lw=1)
-            yaxis_label = r"E$-$E$_\mathrm{F}$ (eV)"
-            print(f"-- Efermi was set to {Ef} eV")
- 
-        if Emin is None: Emin = self.plot_result[:, 1].min() - pad_energy_scale
-        if Emax is None: Emax = self.plot_result[:, 1].max() + pad_energy_scale
-        
-        result = self.plot_result[(self.plot_result[:, 1] >= Emin - max(smear*10, 0.1)) * 
-                                  (self.plot_result[:, 1] <= Emax + max(smear*10, 0.1))]
-
-        # Set weights to 0 which are below threshold_weight
-        if threshold_weight is not None: 
-            result[result[:, -1] < threshold_weight, -1] = 0
-        
-        # Plot as fat band
-        if mode == "fatband":
-            ax = self._plot_fatband(result, ax, marker=marker, fatfactor=fatfactor, 
-                                    scatter_color=color, show_legend=show_legend,
-                                    plotSC=plotSC)
-        elif mode == "density":
-            ax = self._plot_density(result, ax, Emin, Emax, nE, self.kpath_in_angs_, 
-                                    smear, cmap=color_map)
-        elif mode == 'band_centers':
-            ax = self._plot_band_centers(result, ax, color=color, color_map=color_map,
-                                         plot_colormap=plot_colormap_bandcenter)
-        else:
-            raise ValueError("Unknownplot mode: '{}'".format(mode))
-            
-        if special_kpoints is not None:
-            x_tiks_labels, x_tiks_positions = \
-                _FormatSpecialKpts._extract_special_kpts_info(special_kpoints, 
-                                                              self.kpath_in_angs_)
-            plt.xticks(x_tiks_positions, x_tiks_labels)
-            # Draw vertical lines
-            for line_pos in x_tiks_positions:
-                plt.axvline(x=line_pos, color='k', ls='--', lw=2)
-        
-        ax.set_ylabel(yaxis_label)
-        ax.set_ylim([Emin, Emax])
-        ax.set_xlim([self.kpath_in_angs_.min(), self.kpath_in_angs_.max()])
-
-        if save_file_name is None:
-            plt.show()
-        else:
-            CountFig = self.save_figure(save_file_name, CountFig=CountFig)
-            plt.close()
-        return self.fig, ax, CountFig
-    
-    @classmethod
-    def _plot_fatband(cls, data_4_plot, ax, marker='o', fatfactor=20, scatter_color='gray',
-                      cmap='viridis', legend_label='unfolded', show_legend:bool=True,
-                      plotSC:bool=True, legend_pos=1):
-        """
-        Plot fatband scatter plot.
-
-        Parameters
-        ----------
-        data_4_plot : numpy 2d array
-            Data to plot.
-        ax : matplotlib.pyplot axis, optional
-            Figure axis to plot on. 
-        marker : matplotlib.pyplot markerMarkerStyle, optional
-            The marker style. Marker can be either an instance of the class or 
-            the text shorthand for a particular marker. 
-            The default is 'o'.
-        fatfactor : int, optional
-            Scatter plot marker size. The default is 20.
-        scatter_color : str/color, optional
-            Color of plot of unfolded band structure. The color of supercell
-            band structures is gray. The default is 'gray'.
-        cmap : str/ matplotlib colormap
-            Colormap for density plot. The default is 'viridis'.
-        legend_label : str, optional
-            Label to put as legend. The default is 'unfolded'.
-        show_legend : bool, optional
-            If show legend or not. The default is True.
-        plotSC : bool, optional
-            If to plot the supercell band structure. The default is True.
-        legend_pos : TYPE, optional
-            Position of the legend. The default is 1.
-
-        Returns
-        -------
-        ax : matplotlib.pyplot axis
-            Figure axis to plot on. 
-
-        """
-        if plotSC:
-            ax.scatter(data_4_plot[:, 0], data_4_plot[:, 1], s=fatfactor, 
-                       color='gray', label="supercell")
-        ax.scatter(data_4_plot[:, 0], data_4_plot[:, 1], s=data_4_plot[:, 2]*fatfactor, 
-                   marker=marker, color=scatter_color, label=legend_label)
-        if show_legend: 
-            ax.legend(loc=legend_pos)
-        return ax
-     
-    @classmethod              
-    def _plot_density(cls, data_4_plot, ax, Emin, Emax, nE, kpath_in_angs_, 
-                      smear, cmap='viridis'):      
-        """
-        Plot density plot of band structure.
-
-        Parameters
-        ----------
-        data_4_plot : numpy 2d array
-            Data to plot.
-        ax : matplotlib.pyplot axis, optional
-            Figure axis to plot on. 
-        Emin : float
-            Minimum in energy..
-        Emax : float
-            Maximum in energy.
-        nE : int, 
-            Number of pixels in Energy scale when used 'density' mode. 
-        kpath_in_angs_ : array
-            k on path (in A^-1) coordinate. 
-        smear : float
-            Gaussian smearing.
-        cmap : str/ matplotlib colormap
-            Colormap for density plot.The default is 'viridis'.
-
-        Returns
-        -------
-        ax : matplotlib.pyplot axis
-            Figure axis to plot on. 
-
-        """
-        energy = np.linspace(Emin, Emax, nE)
-        density = np.zeros((len(kpath_in_angs_),nE), dtype=float)
-        for k, E, w in data_4_plot[:, :3]:
-            ik = np.argmin(abs(k - kpath_in_angs_))
-            # Gaussian smearing
-            density[ik, :] += w*np.exp(-(energy-E)**2/(2*smear**2)) 
-        # density=np.log(density)
-        # density[density<1e-3]=0           
-        k1 = np.hstack(([kpath_in_angs_[0]], 
-                        (kpath_in_angs_[1:]+kpath_in_angs_[:-1])/2,
-                        [kpath_in_angs_[-1]]))
-        E1 = np.hstack(([energy[0]],(energy[1:]+energy[:-1])/2,[energy[-1]]))
-        # density=np.pad(density,((0,1),(0,1)))
-        # print("before",k1.shape,E1.shape,density.shape)
-        k1, E1 = np.meshgrid(k1,E1)
-        # print("after",k1.shape,E1.shape,density.shape)
-        plt.pcolormesh(k1, E1, density.T, cmap=cmap)
-        plt.colorbar()
-        return ax
-     
-    @classmethod          
-    def _plot_band_centers(cls, data_4_plot, ax, color='k', plot_colormap:bool=True,
-                           err_bar_fmt='x', color_map='viridis'):
-        """
-        Plot the band centers and band width.
-
-        Parameters
-        ----------
-        data_4_plot : numpy 2d array
-            Data to plot.
-        ax : matplotlib.pyplot axis, optional
-            Figure axis to plot on.
-        color : matplotlib color/str, optional
-            Color of the plots. The default is 'k'.
-        plot_colormap : bool, optional
-            If to plot the errorbars as colormap. The default is True.
-        err_bar_fmt : matplotlib errorbar fmt, optional
-            matplotlib errorbar fmt. The default is 'x'.
-        color_map : str/ matplotlib colormap
-            Colormap for density plot.The default is 'viridis'.
-
-        Returns
-        -------
-        ax : matplotlib.pyplot axis
-            Figure axis to plot on. 
-
-        """
-        if plot_colormap:
-            # This is super slow
-            max_weight, min_weight = data_4_plot[:, -1].max(), data_4_plot[:, -1].min()
-            
-            cmap = plt.get_cmap(color_map)  
-            norm = plt.Normalize(min_weight, max_weight)  # Normalize the float values
-            error_colors = cmap(norm(data_4_plot[:, -1]))  # Map float values to colors
-                
-            for ii, JJ in enumerate(data_4_plot):
-                ax.errorbar(JJ[0], JJ[1], yerr=JJ[2], fmt=err_bar_fmt, 
-                            ecolor=error_colors[ii], color=error_colors[ii])
-            cbar = plt.colorbar(plt.cm.ScalarMappable(norm=norm, cmap=cmap), ax=ax)
-            cbar.set_label('Weight')
-        else:
-            ax.errorbar(data_4_plot[:,0], data_4_plot[:,1], yerr=data_4_plot[:, 2], 
-                        fmt=err_bar_fmt, color=color)
+import numpy as np
+import matplotlib.pyplot as plt
+from ..BasicFunctions.general_plot_functions import GeneratePlots
+from .EBS_properties import _FormatSpecialKpts
+
+### ===========================================================================
+
+class EBSplot(GeneratePlots, _FormatSpecialKpts):
+    """
+    Plotting (effective) band structures and related.
+
+    """
+    def __init__(self, kpath_in_angs=None, unfolded_bandstructure=None,
+                 save_figure_dir='.'):
+        """
+        Initialize the band structure plotting class.
+
+        Parameters
+        ----------
+        kpath_in_angs : array, optional
+            k on path (in A^-1) coordinate. The default is None.
+        unfolded_bandstructure : ndarray, optional
+            Unfolded effective band structure data. 
+            Format: k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
+            The default is None.
+        save_figure_dir : str/path, optional
+            Directory where to save the figure. The default is current directory.
+
+        """
+        GeneratePlots.__init__(self, save_figure_dir=save_figure_dir)
+        self.efermi = 0.0
+        
+        if kpath_in_angs is None:
+            try:
+                self.kpath_in_angs_ = self.kpline.copy()
+            except:
+                raise ValueError('No bandstructure data file is found')
+        else:
+            self.kpath_in_angs_ = kpath_in_angs.copy()
+        
+        if unfolded_bandstructure is None:
+            try:
+                self.plot_result = self.unfolded_bandstructure.copy()
+            except:
+                raise ValueError('No bandstructure data file is found')
+        else:
+            self.plot_result = unfolded_bandstructure.copy()
+        
+
+    # def plot(self, ax=None, save_file_name=None, CountFig=None, Ef=None, Emin=None, 
+    #          Emax=None,  pad_energy_scale:float=0.5, threshold_weight:float=None,  
+    #          mode:str="fatband", yaxis_label:str='E (eV)', special_kpoints:dict=None, 
+    #          plotSC:bool=True, marker='o', fatfactor=20, nE:int=100, smear:float=0.05,  
+    #          scatter_color='gray', color_map='viridis', show_legend:bool=True):
+    #     """
+    #     Scatter/density plot of the band structure.
+
+    #     Parameters
+    #     ----------
+    #     ax : matplotlib.pyplot axis, optional
+    #         Figure axis to plot on. If None, new figure will be created.
+    #         The default is None.
+    #     save_file_name : str, optional
+    #         Name of the figure file. If None, figure will be not saved. 
+    #         The default is None.
+    #     CountFig: int, optional
+    #         Figure count. The default is None.
+    #     Ef : float, optional
+    #         Fermi energy. If None, set to 0.0. The default is None.
+    #     Emin : float, optional
+    #         Minimum in energy. The default is None.
+    #     Emax : float, optional
+    #         Maximum in energy. The default is None.
+    #     pad_energy_scale: float, optional
+    #         Add padding of pad_energy_scale to minimum and maximum energy if Emin
+    #         and Emax are None. The default is 0.5.
+    #     threshold_weight : float, optional
+    #         The band centers with band weights lower than the threshhold weights 
+    #         are discarded. The default is None. If None, this is ignored.
+    #     mode : ['fatband','density'], optional
+    #         Mode of plot. The default is "fatband".
+    #     yaxis_label : str, optional
+    #         Y-axis label text. The default is 'E (eV)'.
+    #     special_kpoints : dictionary, optional
+    #         Dictionary of special kpoints position and labels. If None, ignore
+    #         special kpoints. The default is None.
+    #     plotSC : bool, optional
+    #         Plot supercell bandstructure. The default is True.
+    #     marker : matplotlib.pyplot markerMarkerStyle, optional
+    #         The marker style. Marker can be either an instance of the class or 
+    #         the text shorthand for a particular marker. 
+    #         The default is 'o'.
+    #     fatfactor : int, optional
+    #         Scatter plot marker size. The default is 20.
+    #     nE : int, optional
+    #         Number of pixels in Energy scale when used 'density' mode. 
+    #         The default is 100.
+    #     smear : float, optional
+    #         Gaussian smearing. The default is 0.05.
+    #     scatter_color : str/color, optional
+    #         Color of scatter plot of unfolded band structure. The color of supercell
+    #         band structures is gray. The default is 'gray'.
+    #     color_map: str/ matplotlib colormap
+    #         Colormap for density plot. The default is viridis.
+    #     show_legend : bool
+    #         If show legend or not. The default is True.
+        
+    #     Raises
+    #     ------
+    #     ValueError
+    #         If plot mode is unknown.
+
+    #     Returns
+    #     -------
+    #     fig : matplotlib.pyplot.figure
+    #         Figure instance. If ax is not None previously generated fig instance
+    #         will be used.
+    #     ax : Axis instance
+    #         Figure axis instance.
+    #     CountFig: int or None
+    #         Figure count.
+
+    #     """
+        
+    #     print('- Plotting band structures...')
+    #     if ax is None: 
+    #         self.fig, ax = plt.subplots()
+        
+    #     if Ef == 'auto' or Ef is None: 
+    #         Ef = self.efermi
+    #     # Shift the energy scale to 0 fermi energy level   
+    #     if Ef is not None:
+    #         self.plot_result[:,2] -= Ef 
+    #         ax.axhline(y=0, color='k', ls='--', lw=1)
+    #         yaxis_label = r"E$-$E$_\mathrm{F}$ (eV)"
+    #         print(f"-- Efermi was set to {Ef} eV")
+ 
+    #     if Emin is None: Emin = self.plot_result[:,2].min() - pad_energy_scale
+    #     if Emax is None: Emax = self.plot_result[:,2].max() + pad_energy_scale
+        
+    #     result_ = self.plot_result[(self.plot_result[:,2] >= Emin - max(smear*10, 0.1)) * 
+    #                                (self.plot_result[:,2] <= Emax + max(smear*10, 0.1))]
+    #     result = result_[:, 1:]
+    #     # Set weights to 0 which are below threshold_weight
+    #     if threshold_weight is not None: 
+    #         result[result[:, 2] < threshold_weight, 2] = 0
+        
+    #     # Plot as fat band
+    #     if mode == "fatband":
+    #         if plotSC:
+    #             ax.scatter(result[:, 0], result[:, 1], s=fatfactor, color='gray', label="supercell")
+    #         ax.scatter(result[:, 0], result[:, 1], s=result[:, 2]*fatfactor, 
+    #                    marker=marker, color=scatter_color, label="unfolded")
+    #         if show_legend: ax.legend(loc=1)
+    #     elif mode == "density":
+    #         energy = np.linspace(Emin, Emax, nE)
+    #         density = np.zeros((len(self.kpath_in_angs_),nE), dtype=float)
+    #         for k, E, w in result[:, :3]:
+    #             ik = np.argmin(abs(k - self.kpath_in_angs_))
+    #             # Gaussian smearing
+    #             density[ik, :] += w*np.exp(-(energy-E)**2/(2*smear**2)) 
+    #         # density=np.log(density)
+    #         # density[density<1e-3]=0           
+    #         k1 = np.hstack(([self.kpath_in_angs_[0]], 
+    #                         (self.kpath_in_angs_[1:]+self.kpath_in_angs_[:-1])/2,
+    #                         [self.kpath_in_angs_[-1]]))
+    #         E1 = np.hstack(([energy[0]],(energy[1:]+energy[:-1])/2,[energy[-1]]))
+    #         # print(k1,E1)
+    #         # density=np.pad(density,((0,1),(0,1)))
+    #         # print("before",k1.shape,E1.shape,density.shape)
+    #         k1, E1 = np.meshgrid(k1,E1)
+    #         # print("after",k1.shape,E1.shape,density.shape)
+    #         plt.pcolormesh(k1, E1, density.T, cmap=color_map)
+    #         plt.colorbar()
+    #     else:
+    #         raise ValueError("Unknownplot mode: '{}'".format(mode))
+            
+    #     if special_kpoints is not None:
+    #         x_tiks_labels, x_tiks_positions = \
+    #             _FormatSpecialKpts._extract_special_kpts_info(special_kpoints, 
+    #                                                           self.kpath_in_angs_)
+    #         plt.xticks(x_tiks_positions, x_tiks_labels)
+    #         # Draw vertical lines
+    #         for line_pos in x_tiks_positions:
+    #             plt.axvline(x=line_pos, color='k', ls='--', lw=2)
+        
+    #     ax.set_ylabel(yaxis_label)
+    #     ax.set_ylim([Emin, Emax])
+    #     ax.set_xlim([self.kpath_in_angs_.min(), self.kpath_in_angs_.max()])
+
+    #     if save_file_name is None:
+    #         plt.show()
+    #     else:
+    #         CountFig = self.save_figure(save_file_name, CountFig=CountFig)
+    #         plt.close()
+    #     return self.fig, ax, CountFig
+    
+    def plot(self, ax=None, save_file_name=None, CountFig=None, Ef=None, Emin=None, 
+             Emax=None,  pad_energy_scale:float=0.5, threshold_weight:float=None,  
+             mode:str="fatband", yaxis_label:str='E (eV)', special_kpoints:dict=None, 
+             plotSC:bool=True, marker='o', fatfactor=20, nE:int=100, smear:float=0.05,  
+             color='gray', color_map='viridis', plot_colormap_bandcenter:bool=True,
+             show_legend:bool=True):
+        """
+        Scatter/density plot of the band structure.
+
+        Parameters
+        ----------
+        ax : matplotlib.pyplot axis, optional
+            Figure axis to plot on. If None, new figure will be created.
+            The default is None.
+        save_file_name : str, optional
+            Name of the figure file. If None, figure will be not saved. 
+            The default is None.
+        CountFig: int, optional
+            Figure count. The default is None.
+        Ef : float, optional
+            Fermi energy. If None, set to 0.0. The default is None.
+        Emin : float, optional
+            Minimum in energy. The default is None.
+        Emax : float, optional
+            Maximum in energy. The default is None.
+        pad_energy_scale: float, optional
+            Add padding of pad_energy_scale to minimum and maximum energy if Emin
+            and Emax are None. The default is 0.5.
+        threshold_weight : float, optional
+            The band centers with band weights lower than the threshhold weights 
+            are discarded. The default is None. If None, this is ignored.
+        mode : ['fatband','density', 'band_centers'], optional
+            Mode of plot. The default is "fatband".
+        yaxis_label : str, optional
+            Y-axis label text. The default is 'E (eV)'.
+        special_kpoints : dictionary, optional
+            Dictionary of special kpoints position and labels. If None, ignore
+            special kpoints. The default is None.
+        plotSC : bool, optional
+            Plot supercell bandstructure. The default is True.
+        marker : matplotlib.pyplot markerMarkerStyle, optional
+            The marker style. Marker can be either an instance of the class or 
+            the text shorthand for a particular marker. 
+            The default is 'o'.
+        fatfactor : int, optional
+            Scatter plot marker size. The default is 20.
+        nE : int, optional
+            Number of pixels in Energy scale when used 'density' mode. 
+            The default is 100.
+        smear : float, optional
+            Gaussian smearing. The default is 0.05.
+        color : str/color, optional
+            Color of plot of unfolded band structure. The color of supercell
+            band structures is gray. The default is 'gray'.
+        color_map: str/ matplotlib colormap
+            Colormap for density plot. The default is viridis.
+        plot_colormap_bandcenter : bool, optional
+            If plotting the band ceneters by colormap. The default is True.
+        show_legend : bool, optional
+            If show legend or not. The default is True.
+        
+        Raises
+        ------
+        ValueError
+            If plot mode is unknown.
+
+        Returns
+        -------
+        fig : matplotlib.pyplot.figure
+            Figure instance. If ax is not None previously generated fig instance
+            will be used.
+        ax : Axis instance
+            Figure axis instance.
+        CountFig: int or None
+            Figure count.
+
+        """
+        
+        print('- Plotting band structures...')
+        if ax is None: 
+            self.fig, ax = plt.subplots()
+        
+        if mode != "band_centers" and len(self.plot_result[0]) > 3: 
+            self.plot_result = self.plot_result[:, 1:]
+        
+        if Ef == 'auto' or Ef is None: 
+            Ef = self.efermi
+        # Shift the energy scale to 0 fermi energy level   
+        if Ef is not None:
+            self.plot_result[:, 1] -= Ef 
+            ax.axhline(y=0, color='k', ls='--', lw=1)
+            yaxis_label = r"E$-$E$_\mathrm{F}$ (eV)"
+            print(f"-- Efermi was set to {Ef} eV")
+ 
+        if Emin is None: Emin = self.plot_result[:, 1].min() - pad_energy_scale
+        if Emax is None: Emax = self.plot_result[:, 1].max() + pad_energy_scale
+        
+        result = self.plot_result[(self.plot_result[:, 1] >= Emin - max(smear*10, 0.1)) * 
+                                  (self.plot_result[:, 1] <= Emax + max(smear*10, 0.1))]
+
+        # Set weights to 0 which are below threshold_weight
+        if threshold_weight is not None: 
+            result[result[:, -1] < threshold_weight, -1] = 0
+        
+        # Plot as fat band
+        if mode == "fatband":
+            ax = self._plot_fatband(result, ax, marker=marker, fatfactor=fatfactor, 
+                                    scatter_color=color, show_legend=show_legend,
+                                    plotSC=plotSC)
+        elif mode == "density":
+            ax = self._plot_density(result, ax, Emin, Emax, nE, self.kpath_in_angs_, 
+                                    smear, cmap=color_map)
+        elif mode == 'band_centers':
+            ax = self._plot_band_centers(result, ax, color=color, color_map=color_map,
+                                         plot_colormap=plot_colormap_bandcenter)
+        else:
+            raise ValueError("Unknownplot mode: '{}'".format(mode))
+            
+        if special_kpoints is not None:
+            x_tiks_labels, x_tiks_positions = \
+                _FormatSpecialKpts._extract_special_kpts_info(special_kpoints, 
+                                                              self.kpath_in_angs_)
+            plt.xticks(x_tiks_positions, x_tiks_labels)
+            # Draw vertical lines
+            for line_pos in x_tiks_positions:
+                plt.axvline(x=line_pos, color='k', ls='--', lw=2)
+        
+        ax.set_ylabel(yaxis_label)
+        ax.set_ylim([Emin, Emax])
+        ax.set_xlim([self.kpath_in_angs_.min(), self.kpath_in_angs_.max()])
+
+        if save_file_name is None:
+            plt.show()
+        else:
+            CountFig = self.save_figure(save_file_name, CountFig=CountFig)
+            plt.close()
+        return self.fig, ax, CountFig
+    
+    @classmethod
+    def _plot_fatband(cls, data_4_plot, ax, marker='o', fatfactor=20, scatter_color='gray',
+                      cmap='viridis', legend_label='unfolded', show_legend:bool=True,
+                      plotSC:bool=True, legend_pos=1):
+        """
+        Plot fatband scatter plot.
+
+        Parameters
+        ----------
+        data_4_plot : numpy 2d array
+            Data to plot.
+        ax : matplotlib.pyplot axis, optional
+            Figure axis to plot on. 
+        marker : matplotlib.pyplot markerMarkerStyle, optional
+            The marker style. Marker can be either an instance of the class or 
+            the text shorthand for a particular marker. 
+            The default is 'o'.
+        fatfactor : int, optional
+            Scatter plot marker size. The default is 20.
+        scatter_color : str/color, optional
+            Color of plot of unfolded band structure. The color of supercell
+            band structures is gray. The default is 'gray'.
+        cmap : str/ matplotlib colormap
+            Colormap for density plot. The default is 'viridis'.
+        legend_label : str, optional
+            Label to put as legend. The default is 'unfolded'.
+        show_legend : bool, optional
+            If show legend or not. The default is True.
+        plotSC : bool, optional
+            If to plot the supercell band structure. The default is True.
+        legend_pos : TYPE, optional
+            Position of the legend. The default is 1.
+
+        Returns
+        -------
+        ax : matplotlib.pyplot axis
+            Figure axis to plot on. 
+
+        """
+        if plotSC:
+            ax.scatter(data_4_plot[:, 0], data_4_plot[:, 1], s=fatfactor, 
+                       color='gray', label="supercell")
+        ax.scatter(data_4_plot[:, 0], data_4_plot[:, 1], s=data_4_plot[:, 2]*fatfactor, 
+                   marker=marker, color=scatter_color, label=legend_label)
+        if show_legend: 
+            ax.legend(loc=legend_pos)
+        return ax
+     
+    @classmethod              
+    def _plot_density(cls, data_4_plot, ax, Emin, Emax, nE, kpath_in_angs_, 
+                      smear, cmap='viridis'):      
+        """
+        Plot density plot of band structure.
+
+        Parameters
+        ----------
+        data_4_plot : numpy 2d array
+            Data to plot.
+        ax : matplotlib.pyplot axis, optional
+            Figure axis to plot on. 
+        Emin : float
+            Minimum in energy..
+        Emax : float
+            Maximum in energy.
+        nE : int, 
+            Number of pixels in Energy scale when used 'density' mode. 
+        kpath_in_angs_ : array
+            k on path (in A^-1) coordinate. 
+        smear : float
+            Gaussian smearing.
+        cmap : str/ matplotlib colormap
+            Colormap for density plot.The default is 'viridis'.
+
+        Returns
+        -------
+        ax : matplotlib.pyplot axis
+            Figure axis to plot on. 
+
+        """
+        energy = np.linspace(Emin, Emax, nE)
+        density = np.zeros((len(kpath_in_angs_),nE), dtype=float)
+        for k, E, w in data_4_plot[:, :3]:
+            ik = np.argmin(abs(k - kpath_in_angs_))
+            # Gaussian smearing
+            density[ik, :] += w*np.exp(-(energy-E)**2/(2*smear**2)) 
+        # density=np.log(density)
+        # density[density<1e-3]=0           
+        k1 = np.hstack(([kpath_in_angs_[0]], 
+                        (kpath_in_angs_[1:]+kpath_in_angs_[:-1])/2,
+                        [kpath_in_angs_[-1]]))
+        E1 = np.hstack(([energy[0]],(energy[1:]+energy[:-1])/2,[energy[-1]]))
+        # density=np.pad(density,((0,1),(0,1)))
+        # print("before",k1.shape,E1.shape,density.shape)
+        k1, E1 = np.meshgrid(k1,E1)
+        # print("after",k1.shape,E1.shape,density.shape)
+        plt.pcolormesh(k1, E1, density.T, cmap=cmap)
+        plt.colorbar()
+        return ax
+     
+    @classmethod          
+    def _plot_band_centers(cls, data_4_plot, ax, color='k', plot_colormap:bool=True,
+                           err_bar_fmt='x', color_map='viridis'):
+        """
+        Plot the band centers and band width.
+
+        Parameters
+        ----------
+        data_4_plot : numpy 2d array
+            Data to plot.
+        ax : matplotlib.pyplot axis, optional
+            Figure axis to plot on.
+        color : matplotlib color/str, optional
+            Color of the plots. The default is 'k'.
+        plot_colormap : bool, optional
+            If to plot the errorbars as colormap. The default is True.
+        err_bar_fmt : matplotlib errorbar fmt, optional
+            matplotlib errorbar fmt. The default is 'x'.
+        color_map : str/ matplotlib colormap
+            Colormap for density plot.The default is 'viridis'.
+
+        Returns
+        -------
+        ax : matplotlib.pyplot axis
+            Figure axis to plot on. 
+
+        """
+        if plot_colormap:
+            # This is super slow
+            max_weight, min_weight = data_4_plot[:, -1].max(), data_4_plot[:, -1].min()
+            
+            cmap = plt.get_cmap(color_map)  
+            norm = plt.Normalize(min_weight, max_weight)  # Normalize the float values
+            error_colors = cmap(norm(data_4_plot[:, -1]))  # Map float values to colors
+                
+            for ii, JJ in enumerate(data_4_plot):
+                ax.errorbar(JJ[0], JJ[1], yerr=JJ[2], fmt=err_bar_fmt, 
+                            ecolor=error_colors[ii], color=error_colors[ii])
+            cbar = plt.colorbar(plt.cm.ScalarMappable(norm=norm, cmap=cmap), ax=ax)
+            cbar.set_label('Weight')
+        else:
+            ax.errorbar(data_4_plot[:,0], data_4_plot[:,1], yerr=data_4_plot[:, 2], 
+                        fmt=err_bar_fmt, color=color)
         return ax
```

### Comparing `banduppy-0.3.0/banduppy/Utilities/EBS_properties.py` & `banduppy-0.3.1/banduppy/Utilities/EBS_properties.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,570 +1,570 @@
-import numpy as np
-from ..BasicFunctions.general_functions import SaveData2File, _draw_line_length
-
-### ===========================================================================
-class _FormatSpecialKpts:
-    """
-    Find position and format labels of the special k-points.
-
-    """
-    @staticmethod
-    def _extract_special_kpts_info(special_kpts, kpath_angs):
-        """
-        Reform position and labels of special kpoints.
-    
-        Parameters
-        ----------
-        special_kpts : dictionary
-            Dictionary of special kpoints position and labels. If None, ignore
-            special kpoints. 
-        kpath_angs : array
-            k on path (in A^-1) coordinate.
-    
-        Returns
-        -------
-        special_kpts_labels : string list
-            Labels of the special kpoints.
-        special_kpts_poss : float list
-            Positions (in angstrom) of the special kpoints.
-    
-        """
-        kl = np.array([kpath_angs[ik] for ik in special_kpts.keys()])
-        ll = np.array([k for k in special_kpts.values()])
-        borders = [0] + list(np.where((kl[1:]-kl[:-1])>1e-4)[0]+1) + [len(kl)]
-        k_labels=[(kl[b1:b2].mean(),"/".join(set(ll[b1:b2]))) for b1,b2 in zip(borders,borders[1:])]
-        
-        special_kpts_labels = [label[1] for label in k_labels]
-        special_kpts_poss = [label[0] for label in k_labels]
-        return special_kpts_labels, special_kpts_poss
-
-class BandCentersBroadening:
-    """
-    Find band centers and broadening of the unfolded band structure. 
-    The implementation is based on the SCF algorithm of automatic band center 
-    determination from PRB 89, 041407(R) (2014) paper.
-    Original implementation: 
-        https://github.com/band-unfolding/bandup/utils/post_unfolding/
-        locate_band_centers_and_estimate_broadening/find_band_centers_and_broadenings.py
-
-    """
-    def __init__(self, unfolded_bandstructure, min_dN_pre_screening:float=1e-4,
-                 threshold_dN_2b_trial_band_center:float=0.05,
-                 min_sum_dNs_for_a_band:float=0.05, 
-                 precision_pos_band_centers:float=1e-5,
-                 err_tolerance_compare_kpts:float=1e-8,
-                 print_log='low'):
-        """
-        Intializing BandCentersBroadening class. Play with the different cut-offs
-        and threshold values here.
-
-        Parameters
-        ----------
-        unfolded_bandstructure : numpy array
-            Unfolded effective band structure. 
-            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
-        min_dN_pre_screening : float, optional
-            Discard the bands which has weights below min_dN_pre_screening. This
-            pre-screening step helps to minimize the data that will processed
-            now on. The default is 1e-4.
-        threshold_dN_2b_trial_band_center : float, optional
-            Initial guess of the band centers based on the threshold wights. 
-            The default is 0.05.
-        min_sum_dNs_for_a_band : float, optional
-            Cut off criteria for minimum weights that band center should have. 
-            The band centers with lower weights than min_sum_dNs_for_a_band will be
-            discarded during SCF refinements. If min_sum_dNs_for_a_band  
-            is smaller than threshold_dN_2b_trial_band_center, min_sum_dNs_for_a_band
-            will be reset to threshold_dN_2b_trial_band_center value.
-            The default is 0.05.
-        precision_pos_band_centers : float, optional (in eV)
-            Precision when compared band centers from previous and latest SCF
-            iteration. SCF is considered converged if this precision is reached.
-            The default is 1e-5.
-        err_tolerance_compare_kpts : float, optional
-            The tolerance to group the bands set per unique kpoints. 
-            The default is 1e-8.
-        print_log : [None,'low','medium','high'], optional
-            Print information of kpoints folding. Level of printing information. 
-            The default is 'low'. If None, nothing is printed.
-
-        """
-        # Pre-screen band structure data to minimize unnecessary small weights bands
-        self.unfolded_bandstructure_ = self._pre_screen_bandstr_data(unfolded_bandstructure, 
-                                                                     min_dN_pre_screening)
-        
-        # Setting parameters
-        self.prec_pos_band_centers = precision_pos_band_centers
-        self.err_tolerance = err_tolerance_compare_kpts
-        self.print_output = print_log
-        
-        # Reset some parameters based on condition check
-        self.min_sum_dNs_for_each_band, self.threshold_dN_trial_band_center = \
-            self._check_min_sum_dNs_condition(min_sum_dNs_for_a_band, 
-                                              threshold_dN_2b_trial_band_center)
-        
-    def scfs_band_centers_broadening(self, collect_data_scf:bool=False,
-                                     save_data = {'save2file': False, 
-                                                  'fdir': '.',
-                                                  'fname': 'unfolded_bandcenters',
-                                                  'fname_suffix': ''}):
-        """
-        Find the band centers and broadening for a band structure. 
-        The implementation is based on the SCF algorithm of automatic band center 
-        determination from PRB 89, 041407(R) (2014) paper.
-        Original implementation: 
-            https://github.com/band-unfolding/bandup/utils/post_unfolding/
-            locate_band_centers_and_estimate_broadening/find_band_centers_and_broadenings.py
-
-        Parameters
-        ----------
-        collect_data_scf : bool, optional
-            Whether to save the dtails of band centers in each SCF cycles. 
-            The default is False.
-        save_data : dictionary, optional
-            save2file :: Save unfolded kpoints or not? 
-            fir :: str or path
-                Directory path where to save the file.
-            fname :: str
-                Name of the file.
-            fname_suffix :: str
-                Suffix to add to the file name.
-            The default is {'save2file': False, 'fdir': '.', 'fname': 'unfolded_bandcenters', 'fname_suffix': ''}.
-
-        Returns
-        -------
-        return_grouped_unfolded_bandstructure_datails : 2d array
-            Each array contains the final details of band centers at each
-            kpoint. 
-            Format: kpoint coordinate, Band center, Band width, Sum of dN.
-        gather_scf_data_ : dictionary of dictionary of array or None
-            Each array contains the final details of band centers in a particular
-            kpoint. The dictionary then contains the details for each SCF cycles with
-            keys are the SCF cycle number. The highest level dictionary then contains 
-            details for each kpoints with keys are the kpoint indices. Returns None
-            if collect_data_scf is false.
-
-        """
-        print(f"{'-'*72}\n- Finding band center and broadening for band structure...")
-        self.unfolded_bandstructure_ = self._eliminate_duplicate_kpts_list(self.unfolded_bandstructure_)
-        grouped_unfolded_bandstructure = self._group_unique_kpts_data(self.unfolded_bandstructure_,
-                                                                      err_tolerance=self.err_tolerance)
-        gather_scf_data_ = {} if collect_data_scf else None
-        return_grouped_unfolded_bandstructure_datails = []
-        
-        for unfolded_bandstructure_current_kpt in  grouped_unfolded_bandstructure:
-            k_index_i, guess_band_details, all_data_ = \
-                self._scfs_band_centers_broadening_kpt(unfolded_bandstructure_current_kpt,
-                                                       collect_data_scf=collect_data_scf)
-            if collect_data_scf: gather_scf_data_[k_index_i] = all_data_
-            return_grouped_unfolded_bandstructure_datails.append(guess_band_details)
-        print('- Done')   
-        #return return_grouped_unfolded_bandstructure_datails, gather_scf_data_
-        final_results = np.concatenate(return_grouped_unfolded_bandstructure_datails, axis=0)
-        
-        save_data = SaveData2File.default_save_settings(save_data)
-        if save_data['save2file']:
-            self._save_band_centers(data2save=final_results, 
-                                    save_dir=save_data["fdir"], 
-                                    file_name=save_data["fname"], 
-                                    file_name_suffix=save_data["fname_suffix"])       
-        return final_results, gather_scf_data_
-        
-    def _scfs_band_centers_broadening_kpt(self, unfolded_bandstructure_current_kpt,
-                                          collect_data_scf:bool=False):
-        """
-        Find the band centers and broadening for a particular kpoint.
-
-        Parameters
-        ----------
-        unfolded_bandstructure_current_kpt : 2d numpy array
-            Unfolded effective band structure. 
-            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
-        collect_data_scf : bool, optional
-            Whether to save the dtails of band centers in each SCF cycles. 
-            The default is False.
-
-        Returns
-        -------
-        k_index_ : int
-            Index of the kpoint.
-        guess_band_details : 2d numpy array
-            Band center details at the particular kpoint.
-            Format: kpoint coordinate, Band center, Band width, Sum of dN.
-        all_data_ : dict or None
-            Dictionary containing the band center details of all SCF cycles . 
-            Return None if collect_data_scf is False.
-
-        """
-        # Collect kpoint information
-        kpoints_cord = unfolded_bandstructure_current_kpt[0, :2]
-        k_index_ = int(kpoints_cord[0])
-        print (f"{'-'*72}\n- Finding band center for kpoint: {k_index_}")
-        all_data_ = {} if collect_data_scf else None
-        
-        # Collect dNs and energies in array
-        dNs_for_current_kpt = unfolded_bandstructure_current_kpt[:, -1]
-        energies_for_current_kpt = unfolded_bandstructure_current_kpt[:, 2]
-        min_energy, max_energy = min(energies_for_current_kpt), max(energies_for_current_kpt)
-        
-        # Initialize gussed band centers
-        ## Apply threshold dN for trial band center
-        guess_band_centers = energies_for_current_kpt[dNs_for_current_kpt >= 
-                                                      self.threshold_dN_trial_band_center]
-        n_guesses_bc_start = len(guess_band_centers)
-
-        # Run self-consistence loop
-        count = 0
-        converged = False
-        while(not converged):
-            count += 1
-            if self.print_output == 'high': print(f'-- SCF cycle: {count}')
-            guess_band_details = self._calculate_guess_band_details(guess_band_centers, 
-                                                                    min_energy, max_energy,
-                                                                    energies_for_current_kpt, 
-                                                                    dNs_for_current_kpt)
-            refined_band_centers = self._refine_band_centers(guess_band_details, min_energy, 
-                                                             self.min_sum_dNs_for_each_band)
-            converged = self._check_convergence(guess_band_centers, refined_band_centers, 
-                                                self.prec_pos_band_centers)
-            if converged:
-                guess_band_details = self._calculate_guess_band_details(refined_band_centers, 
-                                                                        min_energy, max_energy,
-                                                                        energies_for_current_kpt, 
-                                                                        dNs_for_current_kpt)
-                guess_band_details = guess_band_details[guess_band_details[:, -1] >= 
-                                                        self.min_sum_dNs_for_each_band]
-                guess_band_details = np.insert(guess_band_details, 0, kpoints_cord[1], axis=1)
-                n_guesses_bc_end = len(guess_band_details)
-                if self.print_output == 'high':
-                    print('-- Positions of the band centers converged:')
-                    print(f'\t--- Precision reached: {1000.0 * self.prec_pos_band_centers} meV')
-                    print(f'\t--- Total SCF steps: {count}')
-                    print(f'\t--- Start number of band centers: {n_guesses_bc_start}')
-                    print(f'\t--- Final number of band centers: {n_guesses_bc_end}')
-            else:
-                guess_band_centers = refined_band_centers
-                
-            if collect_data_scf: all_data_[count] = guess_band_details
-        # guess_band_details = (#kpoint coordinate #Band center #Band width #Sum of dN)
-        return k_index_, guess_band_details, all_data_
-    
-    @staticmethod
-    def _check_min_sum_dNs_condition(min_sum_dNs_for_a_band, threshold_dN_2b_trial_band_center):
-        """
-        Checking cut off criteria for minimum weights that band center should have. 
-        The band centers with lower weights than min_sum_dNs_for_a_band will be
-        discarded during SCF refinements. If min_sum_dNs_for_a_band  
-        is smaller than threshold_dN_2b_trial_band_center, min_sum_dNs_for_a_band
-        will be reset to threshold_dN_2b_trial_band_center value.
-
-        Parameters
-        ----------
-        min_sum_dNs_for_a_band : float
-            Cut off criteria for minimum weights that band center should have. 
-            The band centers with lower weights than min_sum_dNs_for_a_band will be
-            discarded during SCF refinements.
-        threshold_dN_2b_trial_band_center : float
-            Initial guess of the band centers based on the threshold wights.
-
-        Returns
-        -------
-        min_sum_dNs_for_a_band : float
-            Cut off criteria for minimum weights that band center should have. 
-            The band centers with lower weights than min_sum_dNs_for_a_band will be
-            discarded during SCF refinements.
-        threshold_dN_2b_trial_band_center : float
-            Initial guess of the band centers based on the threshold wights.
-
-        """
-        threshold_dN_2b_trial_band_center = abs(threshold_dN_2b_trial_band_center)
-        if(abs(min_sum_dNs_for_a_band) < threshold_dN_2b_trial_band_center):
-            min_sum_dNs_for_a_band = threshold_dN_2b_trial_band_center
-            print('- WARNING: Resetting min_sum_dNs_for_a_band because it is smaller than threshold_dN_2b_trial_band_center.')
-        return min_sum_dNs_for_a_band, threshold_dN_2b_trial_band_center
-    
-    @classmethod
-    def _pre_screen_bandstr_data(cls, unfolded_bandstructure, min_dN):
-        """
-        Pre-screen band structure data. Discard unnecessary band centers which
-        has very small weights. This minimizes the search space and improves efficiency.
-
-        Parameters
-        ----------
-        unfolded_bandstructure : 2d numpy array
-            Unfolded effective band structure before removing small weights centers. 
-            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
-        min_dN : float
-            Discard the bands which has weights below min_dN_pre_screening. This
-            pre-screening step helps to minimize the data that will processed
-            now on.
-
-        Returns
-        -------
-        2d numpy array
-            Unfolded effective band structure after removing small weights centers. 
-            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
-
-        """
-        # Pre-screening: get rid of very small weights
-        return unfolded_bandstructure[unfolded_bandstructure[:, -1] >= min_dN]
-
-    @classmethod
-    def _eliminate_duplicate_kpts_list(cls, unfolded_bandstructure):
-        """
-        Eliminating duplicated points from the unfolded band structure data. In
-        the way the band structure data are sorted. 
-        Sort order: first kpts, then energy 
-        e.g.: L-G,G-X -> get rid of two Gs
-
-        Parameters
-        ----------
-        unfolded_bandstructure : 2d numpy array
-            Unfolded effective band structure. 
-            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
-
-        Returns
-        -------
-        unfolded_bandstructure : 2d numpy array
-            Unfolded effective band structure after removing duplicates. 
-            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
-
-        """
-        # Eliminating duplicated points, e.g.: L-G,G-X -> get rid of two Gs
-        # Sort order: kpts, then energy
-        sorted_index_data = np.lexsort((unfolded_bandstructure[:, 2], unfolded_bandstructure[:, 1]))
-        unfolded_bandstructure = unfolded_bandstructure[sorted_index_data]
-        dNs = unfolded_bandstructure[:, -1]
-        for kp_point in range(len(unfolded_bandstructure)-1):
-            kp_en1 = unfolded_bandstructure[kp_point]
-            kp_en2 = unfolded_bandstructure[kp_point + 1]
-            if(kp_en1[1]==kp_en2[1] and kp_en1[2]==kp_en2[2]):
-                dNs[kp_point + 1] = max(kp_en1[3], kp_en2[3]) 
-                dNs[kp_point] = 0.0
-               
-        unfolded_bandstructure[:, -1] = dNs
-        return unfolded_bandstructure
-
-    def _group_unique_kpts_data(cls, unfolded_bandstructure, err_tolerance:float=1e-8):
-        """
-        Group bands at each unique k-points.
-
-        Parameters
-        ----------
-        unfolded_bandstructure : 2d numpy array
-            Unfolded effective band structure. 
-            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
-        err_tolerance : float, optional
-            The tolerance to group the bands set per unique kpoints. 
-            The default is 1e-8.
-
-        Returns
-        -------
-        list
-            List of unfolded effective band structure group by kpoints.
-            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor..
-
-        """
-        # Get unique kpoints coordinate
-        unique_kpts_coords = np.unique(unfolded_bandstructure[:, 1])
-        # Group the rows based on unique values in the specified column
-        return [unfolded_bandstructure[abs(unfolded_bandstructure[:, 1] - val) < err_tolerance] 
-                for val in unique_kpts_coords]
-    
-    @classmethod
-    def _weighted_avg_and_std(cls, values, weights):
-        """
-        Calculate average and variance of list of values. 
-
-        Parameters
-        ----------
-        values : 1d array or list
-            Values to average.
-        weights : 1d array or list
-            Values to use as weights in averaging.
-
-        Returns
-        -------
-        tuple (float, float)
-            (average value, std deviation).
-
-        """
-        average = np.average(values, weights=weights)
-        variance = np.average((values-average)**2, weights=weights) 
-        return (average, np.sqrt(variance))
-    
-    @classmethod
-    def _calculate_possible_energy_width(cls, band_centers, min_energy, max_energy):
-        """
-        Set energy width at each band center.
-
-        Parameters
-        ----------
-        band_centers : float array
-            List of band ceneters.
-        min_energy : float
-            Minimum energy.
-        max_energy : float
-            Maximum energy.
-
-        Returns
-        -------
-        2d numpy array
-            Energy width at each band center [from, to].
-
-        """
-        XX = np.array(band_centers[:-1] + band_centers[1:]) * 0.5
-        # +1.0 makes sure to cover '<guess_energy_width[iband][1]' condition
-        # in calculate_guess_band_details()
-        XX = np.insert(XX, [0, len(XX)], [min_energy, max_energy+1.0]) 
-        return np.stack((XX[:-1], XX[1:]), axis=-1) 
-
-    @classmethod
-    def _calculate_guess_band_details(cls, guess_band_centers, min_energy, max_energy,
-                                      energies_, dNs_):
-        """
-        Calculates band ceneters, band weights, and band width.
-
-        Parameters
-        ----------
-        guess_band_centers : float array
-            List of guessed/refined band ceneters.
-        min_energy : float
-            Minimum energy.
-        max_energy : float
-            Maximum energy.
-        energies_ : float array
-            All bands energies at specific kpoint.
-        dNs_ : float array
-            All band weights at specific kpoint.
-
-        Returns
-        -------
-        2d numpy array
-            Band center details at the particular kpoint.
-            Format: kpoint coordinate, Band center, Band width, Sum of dN.
-
-        """
-        guess_energy_width = cls._calculate_possible_energy_width(guess_band_centers, 
-                                                                  min_energy, max_energy)
-        guess_band_details = [] 
-        for iband in range(len(guess_band_centers)):
-            indices_of_enegies_spread_in_band = \
-                np.argwhere((energies_ >= guess_energy_width[iband][0]) & 
-                            (energies_ < guess_energy_width[iband][1])).flatten()       
-            band_weight_ = np.sum(dNs_[indices_of_enegies_spread_in_band])
-            band_centers_, band_width_ = \
-                cls._weighted_avg_and_std(values=energies_[indices_of_enegies_spread_in_band], 
-                                          weights=dNs_[indices_of_enegies_spread_in_band])
-            # Band center, standard width, weight
-            guess_band_details.append([band_centers_, band_width_, band_weight_])
-            
-        return np.array(guess_band_details)
-
-    @classmethod
-    def _refine_band_centers(cls, guess_band_details, min_energy, min_sum_dNs_for_a_band):
-        """
-        Discard band centers which are too close in energy. Reducing the number 
-        of too close energy values.
-        
-        Discard band centers with
-        abs(e_n,current - e_(n-1),current) < 2*max[band_n_width, band_n-1_width]
-
-        Parameters
-        ----------
-        guess_band_details : 2d numpy array
-            Band center details at the particular kpoint.
-            Format: kpoint coordinate, Band center, Band width, Sum of dN.
-        min_energy : TYPE
-            DESCRIPTION.
-        min_sum_dNs_for_a_band : float
-            Cut off criteria for minimum weights that a band center should have. 
-            The band centers with lower weights than min_sum_dNs_for_a_band will be
-            discarded during SCF refinements.
-
-        Returns
-        -------
-        2d numpy array
-            Band center details at the particular kpoint after refining.
-            Format: kpoint coordinate, Band center, Band width, Sum of dN.
-
-        """
-        refined_band_centers = []
-        for iband in range(len(guess_band_details)):
-            bc, bwidth, b_weight = guess_band_details[iband]
-            previous_bc, previous_bwidth, previous_b_weight = guess_band_details[iband-1]
-            #print(iband, bc, bwidth, b_weight, previous_bc, previous_bwidth, previous_b_weight)
-            valid_bc = False
-            if(b_weight < min_sum_dNs_for_a_band or \
-               abs(bc - previous_bc) < 2.0 * max([bwidth, previous_bwidth])): 
-                try:
-                    if(abs(b_weight / previous_b_weight) > 1.0):
-                        del refined_band_centers[-1]
-                        valid_bc = True
-                except:
-                    pass
-            else:
-                valid_bc = True
-
-            if(valid_bc):
-                refined_band_centers.append(bc)
-        return np.array(refined_band_centers)
-
-    @staticmethod
-    def _check_convergence(old_band_centers, new_band_centers, prec_pos_band_centers):
-        """
-        Check if the two band centers are close. If true, then the band ceneter
-        is considered converged in SCF.
-
-        Parameters
-        ----------
-        old_band_centers : 1d numpy array
-            Previous band centers.
-        new_band_centers : 1d numpy array
-            Refined band centers.
-        prec_pos_band_centers : float
-            Precision when compared band centers from previous and latest SCF
-            iteration. SCF is considered converged if this precision is reached.
-
-        Returns
-        -------
-        bool
-            If two arrays are same or not.
-
-        """
-        return all(abs(old_band_centers[:len(new_band_centers)] - new_band_centers) 
-                   <= prec_pos_band_centers)
-
-    def _save_band_centers(self, data2save, save_dir, file_name, file_name_suffix):
-        """
-        Save unfolded band centers data.
-        Format: kpoint coordinate, Band center, Band width, Sum of dN.
-
-        Parameters
-        ----------
-        data2save : 2d array
-            Data to save.
-        save_dir : str or path
-            Directory path where to save the file.
-        file_name : str
-            Name of the file.
-        file_name_suffix : str
-            Suffix to add to the file name.
-
-        Returns
-        -------
-        None.
-
-        """
-        if self.print_output is not None: 
-            print(f"{'='*_draw_line_length}\n- Saving unfolded band centers to file...")
-        header_msg  = " Unfolded band centers data\n"
-        header_msg += " k on path (A^-1), Band center energy, Band width, Sum of dN\n"
-        # Save the sc-kpoints in file
-        save_f_name = \
-        SaveData2File.save_2_file(data=data2save, 
-                                  save_dir=save_dir, file_name=file_name,
-                                  file_name_suffix=f'{file_name_suffix}.dat', 
-                                  header_txt=header_msg, comments_symbol='#',
-                                  print_log=bool(self.print_output))
-        if self.print_output is not None: 
+import numpy as np
+from ..BasicFunctions.general_functions import SaveData2File, _draw_line_length
+
+### ===========================================================================
+class _FormatSpecialKpts:
+    """
+    Find position and format labels of the special k-points.
+
+    """
+    @staticmethod
+    def _extract_special_kpts_info(special_kpts, kpath_angs):
+        """
+        Reform position and labels of special kpoints.
+    
+        Parameters
+        ----------
+        special_kpts : dictionary
+            Dictionary of special kpoints position and labels. If None, ignore
+            special kpoints. 
+        kpath_angs : array
+            k on path (in A^-1) coordinate.
+    
+        Returns
+        -------
+        special_kpts_labels : string list
+            Labels of the special kpoints.
+        special_kpts_poss : float list
+            Positions (in angstrom) of the special kpoints.
+    
+        """
+        kl = np.array([kpath_angs[ik] for ik in special_kpts.keys()])
+        ll = np.array([k for k in special_kpts.values()])
+        borders = [0] + list(np.where((kl[1:]-kl[:-1])>1e-4)[0]+1) + [len(kl)]
+        k_labels=[(kl[b1:b2].mean(),"/".join(set(ll[b1:b2]))) for b1,b2 in zip(borders,borders[1:])]
+        
+        special_kpts_labels = [label[1] for label in k_labels]
+        special_kpts_poss = [label[0] for label in k_labels]
+        return special_kpts_labels, special_kpts_poss
+
+class BandCentersBroadening:
+    """
+    Find band centers and broadening of the unfolded band structure. 
+    The implementation is based on the SCF algorithm of automatic band center 
+    determination from PRB 89, 041407(R) (2014) paper.
+    Original implementation: 
+        https://github.com/band-unfolding/bandup/utils/post_unfolding/
+        locate_band_centers_and_estimate_broadening/find_band_centers_and_broadenings.py
+
+    """
+    def __init__(self, unfolded_bandstructure, min_dN_pre_screening:float=1e-4,
+                 threshold_dN_2b_trial_band_center:float=0.05,
+                 min_sum_dNs_for_a_band:float=0.05, 
+                 precision_pos_band_centers:float=1e-5,
+                 err_tolerance_compare_kpts:float=1e-8,
+                 print_log='low'):
+        """
+        Intializing BandCentersBroadening class. Play with the different cut-offs
+        and threshold values here.
+
+        Parameters
+        ----------
+        unfolded_bandstructure : numpy array
+            Unfolded effective band structure. 
+            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
+        min_dN_pre_screening : float, optional
+            Discard the bands which has weights below min_dN_pre_screening. This
+            pre-screening step helps to minimize the data that will processed
+            now on. The default is 1e-4.
+        threshold_dN_2b_trial_band_center : float, optional
+            Initial guess of the band centers based on the threshold wights. 
+            The default is 0.05.
+        min_sum_dNs_for_a_band : float, optional
+            Cut off criteria for minimum weights that band center should have. 
+            The band centers with lower weights than min_sum_dNs_for_a_band will be
+            discarded during SCF refinements. If min_sum_dNs_for_a_band  
+            is smaller than threshold_dN_2b_trial_band_center, min_sum_dNs_for_a_band
+            will be reset to threshold_dN_2b_trial_band_center value.
+            The default is 0.05.
+        precision_pos_band_centers : float, optional (in eV)
+            Precision when compared band centers from previous and latest SCF
+            iteration. SCF is considered converged if this precision is reached.
+            The default is 1e-5.
+        err_tolerance_compare_kpts : float, optional
+            The tolerance to group the bands set per unique kpoints. 
+            The default is 1e-8.
+        print_log : [None,'low','medium','high'], optional
+            Print information of kpoints folding. Level of printing information. 
+            The default is 'low'. If None, nothing is printed.
+
+        """
+        # Pre-screen band structure data to minimize unnecessary small weights bands
+        self.unfolded_bandstructure_ = self._pre_screen_bandstr_data(unfolded_bandstructure, 
+                                                                     min_dN_pre_screening)
+        
+        # Setting parameters
+        self.prec_pos_band_centers = precision_pos_band_centers
+        self.err_tolerance = err_tolerance_compare_kpts
+        self.print_output = print_log
+        
+        # Reset some parameters based on condition check
+        self.min_sum_dNs_for_each_band, self.threshold_dN_trial_band_center = \
+            self._check_min_sum_dNs_condition(min_sum_dNs_for_a_band, 
+                                              threshold_dN_2b_trial_band_center)
+        
+    def scfs_band_centers_broadening(self, collect_data_scf:bool=False,
+                                     save_data = {'save2file': False, 
+                                                  'fdir': '.',
+                                                  'fname': 'unfolded_bandcenters',
+                                                  'fname_suffix': ''}):
+        """
+        Find the band centers and broadening for a band structure. 
+        The implementation is based on the SCF algorithm of automatic band center 
+        determination from PRB 89, 041407(R) (2014) paper.
+        Original implementation: 
+            https://github.com/band-unfolding/bandup/utils/post_unfolding/
+            locate_band_centers_and_estimate_broadening/find_band_centers_and_broadenings.py
+
+        Parameters
+        ----------
+        collect_data_scf : bool, optional
+            Whether to save the dtails of band centers in each SCF cycles. 
+            The default is False.
+        save_data : dictionary, optional
+            save2file :: Save unfolded kpoints or not? 
+            fir :: str or path
+                Directory path where to save the file.
+            fname :: str
+                Name of the file.
+            fname_suffix :: str
+                Suffix to add to the file name.
+            The default is {'save2file': False, 'fdir': '.', 'fname': 'unfolded_bandcenters', 'fname_suffix': ''}.
+
+        Returns
+        -------
+        return_grouped_unfolded_bandstructure_datails : 2d array
+            Each array contains the final details of band centers at each
+            kpoint. 
+            Format: kpoint coordinate, Band center, Band width, Sum of dN.
+        gather_scf_data_ : dictionary of dictionary of array or None
+            Each array contains the final details of band centers in a particular
+            kpoint. The dictionary then contains the details for each SCF cycles with
+            keys are the SCF cycle number. The highest level dictionary then contains 
+            details for each kpoints with keys are the kpoint indices. Returns None
+            if collect_data_scf is false.
+
+        """
+        print(f"{'-'*72}\n- Finding band center and broadening for band structure...")
+        self.unfolded_bandstructure_ = self._eliminate_duplicate_kpts_list(self.unfolded_bandstructure_)
+        grouped_unfolded_bandstructure = self._group_unique_kpts_data(self.unfolded_bandstructure_,
+                                                                      err_tolerance=self.err_tolerance)
+        gather_scf_data_ = {} if collect_data_scf else None
+        return_grouped_unfolded_bandstructure_datails = []
+        
+        for unfolded_bandstructure_current_kpt in  grouped_unfolded_bandstructure:
+            k_index_i, guess_band_details, all_data_ = \
+                self._scfs_band_centers_broadening_kpt(unfolded_bandstructure_current_kpt,
+                                                       collect_data_scf=collect_data_scf)
+            if collect_data_scf: gather_scf_data_[k_index_i] = all_data_
+            return_grouped_unfolded_bandstructure_datails.append(guess_band_details)
+        print('- Done')   
+        #return return_grouped_unfolded_bandstructure_datails, gather_scf_data_
+        final_results = np.concatenate(return_grouped_unfolded_bandstructure_datails, axis=0)
+        
+        save_data = SaveData2File.default_save_settings(save_data)
+        if save_data['save2file']:
+            self._save_band_centers(data2save=final_results, 
+                                    save_dir=save_data["fdir"], 
+                                    file_name=save_data["fname"], 
+                                    file_name_suffix=save_data["fname_suffix"])       
+        return final_results, gather_scf_data_
+        
+    def _scfs_band_centers_broadening_kpt(self, unfolded_bandstructure_current_kpt,
+                                          collect_data_scf:bool=False):
+        """
+        Find the band centers and broadening for a particular kpoint.
+
+        Parameters
+        ----------
+        unfolded_bandstructure_current_kpt : 2d numpy array
+            Unfolded effective band structure. 
+            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
+        collect_data_scf : bool, optional
+            Whether to save the dtails of band centers in each SCF cycles. 
+            The default is False.
+
+        Returns
+        -------
+        k_index_ : int
+            Index of the kpoint.
+        guess_band_details : 2d numpy array
+            Band center details at the particular kpoint.
+            Format: kpoint coordinate, Band center, Band width, Sum of dN.
+        all_data_ : dict or None
+            Dictionary containing the band center details of all SCF cycles . 
+            Return None if collect_data_scf is False.
+
+        """
+        # Collect kpoint information
+        kpoints_cord = unfolded_bandstructure_current_kpt[0, :2]
+        k_index_ = int(kpoints_cord[0])
+        print (f"{'-'*72}\n- Finding band center for kpoint: {k_index_}")
+        all_data_ = {} if collect_data_scf else None
+        
+        # Collect dNs and energies in array
+        dNs_for_current_kpt = unfolded_bandstructure_current_kpt[:, -1]
+        energies_for_current_kpt = unfolded_bandstructure_current_kpt[:, 2]
+        min_energy, max_energy = min(energies_for_current_kpt), max(energies_for_current_kpt)
+        
+        # Initialize gussed band centers
+        ## Apply threshold dN for trial band center
+        guess_band_centers = energies_for_current_kpt[dNs_for_current_kpt >= 
+                                                      self.threshold_dN_trial_band_center]
+        n_guesses_bc_start = len(guess_band_centers)
+
+        # Run self-consistence loop
+        count = 0
+        converged = False
+        while(not converged):
+            count += 1
+            if self.print_output == 'high': print(f'-- SCF cycle: {count}')
+            guess_band_details = self._calculate_guess_band_details(guess_band_centers, 
+                                                                    min_energy, max_energy,
+                                                                    energies_for_current_kpt, 
+                                                                    dNs_for_current_kpt)
+            refined_band_centers = self._refine_band_centers(guess_band_details, min_energy, 
+                                                             self.min_sum_dNs_for_each_band)
+            converged = self._check_convergence(guess_band_centers, refined_band_centers, 
+                                                self.prec_pos_band_centers)
+            if converged:
+                guess_band_details = self._calculate_guess_band_details(refined_band_centers, 
+                                                                        min_energy, max_energy,
+                                                                        energies_for_current_kpt, 
+                                                                        dNs_for_current_kpt)
+                guess_band_details = guess_band_details[guess_band_details[:, -1] >= 
+                                                        self.min_sum_dNs_for_each_band]
+                guess_band_details = np.insert(guess_band_details, 0, kpoints_cord[1], axis=1)
+                n_guesses_bc_end = len(guess_band_details)
+                if self.print_output == 'high':
+                    print('-- Positions of the band centers converged:')
+                    print(f'\t--- Precision reached: {1000.0 * self.prec_pos_band_centers} meV')
+                    print(f'\t--- Total SCF steps: {count}')
+                    print(f'\t--- Start number of band centers: {n_guesses_bc_start}')
+                    print(f'\t--- Final number of band centers: {n_guesses_bc_end}')
+            else:
+                guess_band_centers = refined_band_centers
+                
+            if collect_data_scf: all_data_[count] = guess_band_details
+        # guess_band_details = (#kpoint coordinate #Band center #Band width #Sum of dN)
+        return k_index_, guess_band_details, all_data_
+    
+    @staticmethod
+    def _check_min_sum_dNs_condition(min_sum_dNs_for_a_band, threshold_dN_2b_trial_band_center):
+        """
+        Checking cut off criteria for minimum weights that band center should have. 
+        The band centers with lower weights than min_sum_dNs_for_a_band will be
+        discarded during SCF refinements. If min_sum_dNs_for_a_band  
+        is smaller than threshold_dN_2b_trial_band_center, min_sum_dNs_for_a_band
+        will be reset to threshold_dN_2b_trial_band_center value.
+
+        Parameters
+        ----------
+        min_sum_dNs_for_a_band : float
+            Cut off criteria for minimum weights that band center should have. 
+            The band centers with lower weights than min_sum_dNs_for_a_band will be
+            discarded during SCF refinements.
+        threshold_dN_2b_trial_band_center : float
+            Initial guess of the band centers based on the threshold wights.
+
+        Returns
+        -------
+        min_sum_dNs_for_a_band : float
+            Cut off criteria for minimum weights that band center should have. 
+            The band centers with lower weights than min_sum_dNs_for_a_band will be
+            discarded during SCF refinements.
+        threshold_dN_2b_trial_band_center : float
+            Initial guess of the band centers based on the threshold wights.
+
+        """
+        threshold_dN_2b_trial_band_center = abs(threshold_dN_2b_trial_band_center)
+        if(abs(min_sum_dNs_for_a_band) < threshold_dN_2b_trial_band_center):
+            min_sum_dNs_for_a_band = threshold_dN_2b_trial_band_center
+            print('- WARNING: Resetting min_sum_dNs_for_a_band because it is smaller than threshold_dN_2b_trial_band_center.')
+        return min_sum_dNs_for_a_band, threshold_dN_2b_trial_band_center
+    
+    @classmethod
+    def _pre_screen_bandstr_data(cls, unfolded_bandstructure, min_dN):
+        """
+        Pre-screen band structure data. Discard unnecessary band centers which
+        has very small weights. This minimizes the search space and improves efficiency.
+
+        Parameters
+        ----------
+        unfolded_bandstructure : 2d numpy array
+            Unfolded effective band structure before removing small weights centers. 
+            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
+        min_dN : float
+            Discard the bands which has weights below min_dN_pre_screening. This
+            pre-screening step helps to minimize the data that will processed
+            now on.
+
+        Returns
+        -------
+        2d numpy array
+            Unfolded effective band structure after removing small weights centers. 
+            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
+
+        """
+        # Pre-screening: get rid of very small weights
+        return unfolded_bandstructure[unfolded_bandstructure[:, -1] >= min_dN]
+
+    @classmethod
+    def _eliminate_duplicate_kpts_list(cls, unfolded_bandstructure):
+        """
+        Eliminating duplicated points from the unfolded band structure data. In
+        the way the band structure data are sorted. 
+        Sort order: first kpts, then energy 
+        e.g.: L-G,G-X -> get rid of two Gs
+
+        Parameters
+        ----------
+        unfolded_bandstructure : 2d numpy array
+            Unfolded effective band structure. 
+            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
+
+        Returns
+        -------
+        unfolded_bandstructure : 2d numpy array
+            Unfolded effective band structure after removing duplicates. 
+            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
+
+        """
+        # Eliminating duplicated points, e.g.: L-G,G-X -> get rid of two Gs
+        # Sort order: kpts, then energy
+        sorted_index_data = np.lexsort((unfolded_bandstructure[:, 2], unfolded_bandstructure[:, 1]))
+        unfolded_bandstructure = unfolded_bandstructure[sorted_index_data]
+        dNs = unfolded_bandstructure[:, -1]
+        for kp_point in range(len(unfolded_bandstructure)-1):
+            kp_en1 = unfolded_bandstructure[kp_point]
+            kp_en2 = unfolded_bandstructure[kp_point + 1]
+            if(kp_en1[1]==kp_en2[1] and kp_en1[2]==kp_en2[2]):
+                dNs[kp_point + 1] = max(kp_en1[3], kp_en2[3]) 
+                dNs[kp_point] = 0.0
+               
+        unfolded_bandstructure[:, -1] = dNs
+        return unfolded_bandstructure
+
+    def _group_unique_kpts_data(cls, unfolded_bandstructure, err_tolerance:float=1e-8):
+        """
+        Group bands at each unique k-points.
+
+        Parameters
+        ----------
+        unfolded_bandstructure : 2d numpy array
+            Unfolded effective band structure. 
+            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
+        err_tolerance : float, optional
+            The tolerance to group the bands set per unique kpoints. 
+            The default is 1e-8.
+
+        Returns
+        -------
+        list
+            List of unfolded effective band structure group by kpoints.
+            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor..
+
+        """
+        # Get unique kpoints coordinate
+        unique_kpts_coords = np.unique(unfolded_bandstructure[:, 1])
+        # Group the rows based on unique values in the specified column
+        return [unfolded_bandstructure[abs(unfolded_bandstructure[:, 1] - val) < err_tolerance] 
+                for val in unique_kpts_coords]
+    
+    @classmethod
+    def _weighted_avg_and_std(cls, values, weights):
+        """
+        Calculate average and variance of list of values. 
+
+        Parameters
+        ----------
+        values : 1d array or list
+            Values to average.
+        weights : 1d array or list
+            Values to use as weights in averaging.
+
+        Returns
+        -------
+        tuple (float, float)
+            (average value, std deviation).
+
+        """
+        average = np.average(values, weights=weights)
+        variance = np.average((values-average)**2, weights=weights) 
+        return (average, np.sqrt(variance))
+    
+    @classmethod
+    def _calculate_possible_energy_width(cls, band_centers, min_energy, max_energy):
+        """
+        Set energy width at each band center.
+
+        Parameters
+        ----------
+        band_centers : float array
+            List of band ceneters.
+        min_energy : float
+            Minimum energy.
+        max_energy : float
+            Maximum energy.
+
+        Returns
+        -------
+        2d numpy array
+            Energy width at each band center [from, to].
+
+        """
+        XX = np.array(band_centers[:-1] + band_centers[1:]) * 0.5
+        # +1.0 makes sure to cover '<guess_energy_width[iband][1]' condition
+        # in calculate_guess_band_details()
+        XX = np.insert(XX, [0, len(XX)], [min_energy, max_energy+1.0]) 
+        return np.stack((XX[:-1], XX[1:]), axis=-1) 
+
+    @classmethod
+    def _calculate_guess_band_details(cls, guess_band_centers, min_energy, max_energy,
+                                      energies_, dNs_):
+        """
+        Calculates band ceneters, band weights, and band width.
+
+        Parameters
+        ----------
+        guess_band_centers : float array
+            List of guessed/refined band ceneters.
+        min_energy : float
+            Minimum energy.
+        max_energy : float
+            Maximum energy.
+        energies_ : float array
+            All bands energies at specific kpoint.
+        dNs_ : float array
+            All band weights at specific kpoint.
+
+        Returns
+        -------
+        2d numpy array
+            Band center details at the particular kpoint.
+            Format: kpoint coordinate, Band center, Band width, Sum of dN.
+
+        """
+        guess_energy_width = cls._calculate_possible_energy_width(guess_band_centers, 
+                                                                  min_energy, max_energy)
+        guess_band_details = [] 
+        for iband in range(len(guess_band_centers)):
+            indices_of_enegies_spread_in_band = \
+                np.argwhere((energies_ >= guess_energy_width[iband][0]) & 
+                            (energies_ < guess_energy_width[iband][1])).flatten()       
+            band_weight_ = np.sum(dNs_[indices_of_enegies_spread_in_band])
+            band_centers_, band_width_ = \
+                cls._weighted_avg_and_std(values=energies_[indices_of_enegies_spread_in_band], 
+                                          weights=dNs_[indices_of_enegies_spread_in_band])
+            # Band center, standard width, weight
+            guess_band_details.append([band_centers_, band_width_, band_weight_])
+            
+        return np.array(guess_band_details)
+
+    @classmethod
+    def _refine_band_centers(cls, guess_band_details, min_energy, min_sum_dNs_for_a_band):
+        """
+        Discard band centers which are too close in energy. Reducing the number 
+        of too close energy values.
+        
+        Discard band centers with
+        abs(e_n,current - e_(n-1),current) < 2*max[band_n_width, band_n-1_width]
+
+        Parameters
+        ----------
+        guess_band_details : 2d numpy array
+            Band center details at the particular kpoint.
+            Format: kpoint coordinate, Band center, Band width, Sum of dN.
+        min_energy : TYPE
+            DESCRIPTION.
+        min_sum_dNs_for_a_band : float
+            Cut off criteria for minimum weights that a band center should have. 
+            The band centers with lower weights than min_sum_dNs_for_a_band will be
+            discarded during SCF refinements.
+
+        Returns
+        -------
+        2d numpy array
+            Band center details at the particular kpoint after refining.
+            Format: kpoint coordinate, Band center, Band width, Sum of dN.
+
+        """
+        refined_band_centers = []
+        for iband in range(len(guess_band_details)):
+            bc, bwidth, b_weight = guess_band_details[iband]
+            previous_bc, previous_bwidth, previous_b_weight = guess_band_details[iband-1]
+            #print(iband, bc, bwidth, b_weight, previous_bc, previous_bwidth, previous_b_weight)
+            valid_bc = False
+            if(b_weight < min_sum_dNs_for_a_band or \
+               abs(bc - previous_bc) < 2.0 * max([bwidth, previous_bwidth])): 
+                try:
+                    if(abs(b_weight / previous_b_weight) > 1.0):
+                        del refined_band_centers[-1]
+                        valid_bc = True
+                except:
+                    pass
+            else:
+                valid_bc = True
+
+            if(valid_bc):
+                refined_band_centers.append(bc)
+        return np.array(refined_band_centers)
+
+    @staticmethod
+    def _check_convergence(old_band_centers, new_band_centers, prec_pos_band_centers):
+        """
+        Check if the two band centers are close. If true, then the band ceneter
+        is considered converged in SCF.
+
+        Parameters
+        ----------
+        old_band_centers : 1d numpy array
+            Previous band centers.
+        new_band_centers : 1d numpy array
+            Refined band centers.
+        prec_pos_band_centers : float
+            Precision when compared band centers from previous and latest SCF
+            iteration. SCF is considered converged if this precision is reached.
+
+        Returns
+        -------
+        bool
+            If two arrays are same or not.
+
+        """
+        return all(abs(old_band_centers[:len(new_band_centers)] - new_band_centers) 
+                   <= prec_pos_band_centers)
+
+    def _save_band_centers(self, data2save, save_dir, file_name, file_name_suffix):
+        """
+        Save unfolded band centers data.
+        Format: kpoint coordinate, Band center, Band width, Sum of dN.
+
+        Parameters
+        ----------
+        data2save : 2d array
+            Data to save.
+        save_dir : str or path
+            Directory path where to save the file.
+        file_name : str
+            Name of the file.
+        file_name_suffix : str
+            Suffix to add to the file name.
+
+        Returns
+        -------
+        None.
+
+        """
+        if self.print_output is not None: 
+            print(f"{'='*_draw_line_length}\n- Saving unfolded band centers to file...")
+        header_msg  = " Unfolded band centers data\n"
+        header_msg += " k on path (A^-1), Band center energy, Band width, Sum of dN\n"
+        # Save the sc-kpoints in file
+        save_f_name = \
+        SaveData2File.save_2_file(data=data2save, 
+                                  save_dir=save_dir, file_name=file_name,
+                                  file_name_suffix=f'{file_name_suffix}.dat', 
+                                  header_txt=header_msg, comments_symbol='#',
+                                  print_log=bool(self.print_output))
+        if self.print_output is not None: 
             print(f'-- Filepath: {save_f_name}\n- Done')
```

### Comparing `banduppy-0.3.0/banduppy/Utilities/folding_degree_plot.py` & `banduppy-0.3.1/banduppy/Utilities/folding_degree_plot.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import numpy as np
-import matplotlib.pyplot as plt
-from ..BasicFunctions.general_plot_functions import GeneratePlots
-
-### ===========================================================================
-
-class FoldingDegreePlot(GeneratePlots):
-    """
-    Plotting number of kpoints in k-path vs degree of folding.
-
-    """
-    def __init__(self, fold_results_dictionary, save_figure_dir='.'):
-        """
-        Initialize the FoldingDegreePlot plotting class.
-
-        Parameters
-        ----------
-        fold_results_dictionary : dictionary
-            Keys are the index of path segment searched from the pathPBZ list supplied.
-            Values are 2d array with each row containing number of division in the 1st
-            column and percent of folding in the 2nd column.
-        save_figure_dir : str/path, optional
-            Directory where to save the figure. The default is current directory.
-
-        """
-        GeneratePlots.__init__(self, save_figure_dir=save_figure_dir)
-        self.proposed_folding_results_ = fold_results_dictionary.copy()
-            
-    def plot_folding(self, save_file_name=None, CountFig=None, yaxis_label:str='Folding degree (%)',
-                     xaxis_label:str='number of kpoints', line_color='k'):
-        
-        print('- Plotting folding degree...')
-        for keys, vals in self.proposed_folding_results_.items():
-            fig, ax = plt.subplots()
-            ax.set_xlabel(xaxis_label)
-            ax.set_ylabel(yaxis_label)
-            
-            path_start, path_end = vals[0]
-            ax.set_title(f'{path_start} --> {path_end}')
-            
-            XX, YY = vals[1][:,0], vals[1][:,1]
-            
-            ax.plot(XX, YY, 'o-', color=line_color)
-        print('- Done...')
-        if save_file_name is None:
-            plt.show()
-        else:
-            CountFig = self.save_figure(save_file_name, CountFig=CountFig)
-            plt.close()
+import numpy as np
+import matplotlib.pyplot as plt
+from ..BasicFunctions.general_plot_functions import GeneratePlots
+
+### ===========================================================================
+
+class FoldingDegreePlot(GeneratePlots):
+    """
+    Plotting number of kpoints in k-path vs degree of folding.
+
+    """
+    def __init__(self, fold_results_dictionary, save_figure_dir='.'):
+        """
+        Initialize the FoldingDegreePlot plotting class.
+
+        Parameters
+        ----------
+        fold_results_dictionary : dictionary
+            Keys are the index of path segment searched from the pathPBZ list supplied.
+            Values are 2d array with each row containing number of division in the 1st
+            column and percent of folding in the 2nd column.
+        save_figure_dir : str/path, optional
+            Directory where to save the figure. The default is current directory.
+
+        """
+        GeneratePlots.__init__(self, save_figure_dir=save_figure_dir)
+        self.proposed_folding_results_ = fold_results_dictionary.copy()
+            
+    def plot_folding(self, save_file_name=None, CountFig=None, yaxis_label:str='Folding degree (%)',
+                     xaxis_label:str='number of kpoints', line_color='k'):
+        
+        print('- Plotting folding degree...')
+        for keys, vals in self.proposed_folding_results_.items():
+            fig, ax = plt.subplots()
+            ax.set_xlabel(xaxis_label)
+            ax.set_ylabel(yaxis_label)
+            
+            path_start, path_end = vals[0]
+            ax.set_title(f'{path_start} --> {path_end}')
+            
+            XX, YY = vals[1][:,0], vals[1][:,1]
+            
+            ax.plot(XX, YY, 'o-', color=line_color)
+        print('- Done...')
+        if save_file_name is None:
+            plt.show()
+        else:
+            CountFig = self.save_figure(save_file_name, CountFig=CountFig)
+            plt.close()
         return fig, ax, CountFig
```

### Comparing `banduppy-0.3.0/banduppy/src/folding.py` & `banduppy-0.3.1/banduppy/src/folding.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,721 +1,721 @@
-import numpy as np
-from ..BasicFunctions.general_functions import SaveData2File, _BasicFunctionsModule, _draw_line_length
-from .folding_properties import FindProperties
-from .. import __version__
-    
-try:
-    from collections.abc import Iterable
-except ImportError:
-    from collections import Iterable
-    
-## ============================================================================    
-class _KpointsModule:   
-    
-    @staticmethod
-    def _find_K_from_k(k, transformation_matrix):
-        """
-        Generate list of SC K-vectors onto which the PC k-vectors folds. 
-        
-            K = k.P
-
-        Parameters
-        ----------
-        k : ndarray of floats
-            PC kpoints.
-        transformation_matrix : ndarray
-            PC to SC transformation matrix.
-
-        Returns
-        -------
-        ndarray of floats
-            SC kpoints.
-
-        """
-        return np.dot(k, transformation_matrix.T)
-
-    @classmethod   
-    def _remove_duplicate_kpoints(cls, kpoints, sort_kpts:bool=False, 
-                                  return_id_mapping:bool=True, decimals:int=10):
-        """
-        Remove duplicate kpoints.
-
-        Parameters
-        ----------
-        kpoints : ndarray of floats
-            kpoints list.
-        sort_kpts : bool, optional
-            Sort the kpoints. The default is False.
-        return_id_mapping : bool, optional
-            Return the id of reverse mapping. The default is True.
-        decimals : int, optional
-            How many decomal points to round up. The default is 10.
-
-        Returns
-        -------
-        ndarray of floats, ndarray of int
-            Reduced kpoint list.
-
-        """
-        kpoints = np.asarray(kpoints)
-        unique_kpts, unique_kpts_ids, kpts_ids = np.unique(_BasicFunctionsModule._return_mod(kpoints),
-                                                           axis=0, return_index=True, return_inverse=True)
-        
-        if sort_kpts:
-            sort_pos_kpts = np.argsort(unique_kpts_ids)
-            unique_kpts_ids = unique_kpts_ids[sort_pos_kpts]
-            unique_kpts = kpoints[unique_kpts_ids]
-            kpts_ids = kpts_ids[sort_pos_kpts]
-
-        if return_id_mapping:
-            return unique_kpts, kpts_ids
-        else:
-            return unique_kpts
-    
-    @classmethod
-    def _search_folding_percent_brute_force(cls, transformation_matrix, start, end, 
-                                            min_div_points, max_div_points):  
-        """
-        Calculates SC Kpoints from PC kpoints and returns percent of folding.
-        This method uses brute force to calculate folding degree i.e. complete
-        list of SC Kpoints are generated in the process. 
-        (Loop over nkpoints in the path segment starting with min_div_points until
-        max_div_points with increment of 1.)
-        
-        Folding percent = ((#of PC kpoints - #of folded SC Kpoints)/(#of PC kpoints))*100
-
-        Parameters
-        ----------
-        transformation_matrix : ndarray
-            PC to SC transformation matrix.
-        start : 1d array
-            Starting coordinate of kpoints path.
-        end : 1d array
-            End coordinate of kpoints path.
-        min_div_points : int
-            Minimum number of kpoints division in the k-path.
-        max_div_points : int
-            Maximum number of kpoints division in the k-path.
-
-        Returns
-        -------
-        numpy ndarray
-            2d array with each row containing number of division in the 1st
-            column and percent of folding in the 2nd column.
-
-        """
-        folding_info_list = []
-        # Loop over nkpoints in the path segment starting with min_div_points until
-        # max_div_points with increment of 1.
-        for div_points in range(min_div_points, max_div_points): 
-            len_unique_Kpts = \
-            len(cls._remove_duplicate_kpoints(
-                _KpointsModule._find_K_from_k(np.linspace(start, end, div_points), 
-                                                            transformation_matrix),
-                sort_kpts=False, return_id_mapping=False))
-            
-            folding_info_list.append([div_points, 
-                                      (div_points-len_unique_Kpts)/div_points*100]) 
-        return np.array(folding_info_list)
-
-    @classmethod           
-    def _serach_max_min_folding(cls, transformation_matrix, start, end, 
-                                min_num_pts:int=5, max_num_pts:int=20,
-                                serach_mode:str='brute_force'):
-        """
-        Calculates SC Kpoints from PC kpoints and returns percent of folding.
-        Maximum and Minimum degree of folding are reported.
-        
-        Folding percent = ((#of PC kpoints - #of folded SC Kpoints)/(#of PC kpoints))*100
-
-        Parameters
-        ----------
-        transformation_matrix : ndarray
-            PC to SC transformation matrix.
-        start : 1d array
-            Starting coordinate of kpoints path.
-        end : 1d array
-            End coordinate of kpoints path.
-        min_num_pts : int, optional
-            Minimum number of kpoints division in the k-path. The default is 5.
-        max_num_pts : int, optional
-            Maximum number of kpoints division in the k-path. The default is 20.
-        serach_mode : ['brute_force'], optional
-            Method to calculate SC Kpoints. The default is 'brute_force'.
-
-        Returns
-        -------
-        folding_data_ : numpy ndarray
-            2d array with each row containing number of division in the 1st
-            column and percent of folding in the 2nd column.
-
-        """
-        assert max_num_pts >= min_num_pts, f'max_num_pts should be >= min_num_pts {min_num_pts}.'
-        if serach_mode == 'brute_force':
-            folding_data_ = cls._search_folding_percent_brute_force(transformation_matrix, 
-                                                                    start, end, 
-                                                                    min_num_pts, max_num_pts)
-            max_folding = folding_data_[np.argmax(folding_data_[:,1])]
-            min_folding = folding_data_[np.argmin(folding_data_[:,1])]
-            print(f'--- Maximum folding (nkpts, folding percent): {int(max_folding[0]):>3d}, {max_folding[1]:.3f}%')
-            print(f'--- Minimum folding (nkpts, folding percent): {int(min_folding[0]):>3d}, {min_folding[1]:.3f}%')
-            return folding_data_ 
-        
-    @classmethod           
-    def _propose_max_min_folding(cls, transformation_matrix, pathPBZ, 
-                                 min_num_pts:int=5, max_num_pts:int=20,
-                                 serach_mode:str='brute_force'):
-        """
-        Calculates SC Kpoints from PC kpoints and returns percent of folding.
-        Maximum and Minimum degree of folding are reported.
-        
-        Folding percent = ((#of PC kpoints - #of folded SC Kpoints)/(#of PC kpoints))*100
-
-        Parameters
-        ----------
-        transformation_matrix : ndarray
-            PC to SC transformation matrix.
-        pathPBZ : ndarray/list
-            PC kpoint path nodes in reduced coordinates.
-        min_num_pts : int, optional
-            Minimum number of kpoints division in the k-path. The default is 5.
-        max_num_pts : int, optional
-            Maximum number of kpoints division in the k-path. The default is 20.
-        serach_mode : ['brute_force'], optional
-            Method to calculate SC Kpoints. The default is 'brute_force'.
-
-        Returns
-        -------
-        propose_folding_data_ : dictionary
-            {index: ((start node, end node), folding data)}
-            index : Index of path segment searched from the pathPBZ list supplied.
-            folding data : 2d array with each row containing number of division in the 1st
-            column and percent of folding in the 2nd column.
-
-        """
-        propose_folding_data_ = {}
-        print(f"{'='*_draw_line_length}\n- Proposing maximum and minimum band folding...")
-        # Iterate over the list, skipping the last element
-        for i in range(len(pathPBZ) - 1):
-            # Check if both current and next elements are not None
-            if pathPBZ[i] is not None and pathPBZ[i + 1] is not None:
-                # Get start and end of k-path segment
-                start, end = np.array(pathPBZ[i]), np.array(pathPBZ[i + 1])
-                assert start.shape == end.shape == (3,)
-                print(f'-- k-path: {start} --> {end}')
-                # Search for max-min folding
-                propose_folding_data_[i] = ((start, end),
-                    cls._serach_max_min_folding(transformation_matrix, start, end, 
-                                                                       min_num_pts=min_num_pts, 
-                                                                       max_num_pts=max_num_pts,
-                                                                       serach_mode=serach_mode))
-        return propose_folding_data_
-
-        
-    @staticmethod   
-    def _generate_kpts_from_kpath(pathPBZ, nk, labels):
-        """
-        Creates
-
-        Parameters
-        ----------
-        pathPBZ : ndarray/list, optional
-            PC kpoint path nodes in reduced coordinates. 
-        nk : int ot tuple, optional
-            Number of kpoints in each k-path segment. 
-        labels : string ot list of strings
-            Labels of special k-points, either as a continuous list or string. 
-            Do not use ',' or multidimentional list do define disjoint segmants.
-            e.g. Do not use labels='LG,KG'. Use labels='LGKG'. The 'None' in the
-            pathPBZ will take care of the disjoint segments.
-            If multiple word needs to be single label, use list.
-            e.g. labels=['X','Gamma','L']. Do not use string labels='XGammaL'.
-            If None, the special kpoints will be indexed as 1,2,3,...
-
-        Returns
-        -------
-        kpointsPBZ : ndarray, optional
-            PC kpoint list. 
-        special_kpoints_pos_labels : dictionary
-            Special k-points position and labels.
-
-        """
-        # List of number_of_kpoints in segment
-        # Convert nk to generator if it's iterable
-        nkgen = (x for x in nk) if isinstance(nk, Iterable) else (nk for _ in pathPBZ)
-        
-        # Total nodes in the PC BZ supplied
-        total_k_nodes = len([1 for k in pathPBZ if k is not None])
-        
-        # Create labels list for special_kpoints_labels
-        if labels is None:
-            labels = [str(i+1) for i in range(total_k_nodes)]
-        else:
-            assert len(labels) >= total_k_nodes , 'Number of labels is less than the supplied k-path segments.'
-        labels = (l for l in labels)
-        labels = [None if k is None else next(labels) for k in pathPBZ]
-        
-        # Initialize
-        kpointsPBZ=np.zeros((0,3))
-        special_kpoints_pos_labels={}
-        
-        # Iterate over the list, skipping the last element
-        for i in range(len(pathPBZ) - 1):
-            # Check if both current and next elements are not None
-            if pathPBZ[i] is not None and pathPBZ[i + 1] is not None:
-                # Get position of special k-point for plotting later
-                special_kpoints_pos_labels[kpointsPBZ.shape[0]] = labels[i]
-                # Get start and end of k-path segment
-                start, end = np.array(pathPBZ[i]), np.array(pathPBZ[i + 1])
-                assert start.shape == end.shape == (3,)
-                # Get nk in k-path segment
-                try:
-                    num_points = next(nkgen)
-                except: 
-                    raise StopIteration('Number of nk is less than the supplied k-path segments.')
-                # Generate k-points using linspace
-                interpolated_points = np.linspace(start, end, num_points)
-                kpointsPBZ = np.vstack((kpointsPBZ, interpolated_points))
-                # Get position of special k-point for plotting later
-                special_kpoints_pos_labels[kpointsPBZ.shape[0] - 1] = labels[i+1] 
-    
-        return kpointsPBZ, special_kpoints_pos_labels, nkgen, labels
-    
-    @staticmethod
-    def _pad_kpts_weights(kpoints, kpts_weights=1):
-        """
-        Padding the weights of SC kpoints.
-
-        Parameters
-        ----------
-        kpoints : ndarray of floats
-            kpoints list.
-        kpts_weights : int or float or 1d numpy array, optional
-            Weights of the SC kpoints. The default is 1.
-
-        Returns
-        -------
-        ndarray of floats
-            kpoints list padded with weights.
-
-        """
-
-        if isinstance(kpts_weights, int) or isinstance(kpts_weights, float):
-            append_weights = np.array([[kpts_weights]*len(kpoints)])
-        else:
-            append_weights = np.copy([kpts_weights])
-        return np.concatenate((kpoints, append_weights.T), axis=1)
-    
-    @staticmethod
-    def _generate_foot_text(pc_kpoints_list, labels=None, nk_list=None):
-        """
-        Create foorter text for the SC kpoints save file.
-
-        Parameters
-        ----------
-        pc_kpoints_list : ndarray/list
-            List of PC kpoints or k-path.
-        labels : list, optional
-            List of special k-points in k-path. The default is None.
-        nk_list : list, optional
-            List of number of k-points in each k-path segments. The default is None.
-
-        Returns
-        -------
-        append_foot_file : str
-            Text string for footer of save file.
-
-        """
-        append_foot_file  = '\n\n! The above SCKPTS (and/or some other SCKPTS related to them by symm. ops. of the SCBZ)'
-        append_foot_file += '\n! unfold onto the pckpts listed below (selected by you):'
-        append_foot_file += '\n! k-points for PC bandstructure '
-        # Add label texts
-        if labels is not None:                   
-            append_foot_file += ','.join('-'.join(label for label in group_ if label) 
-                                         for group_ in ''.join(str(label) for label in labels).split('None') if group_)         
-        # Add number of kpoints in each segment
-        if nk_list is not None: 
-            if not isinstance(nk_list, Iterable): nk_list = [nk_list]
-            append_foot_file += '\n! '
-            append_foot_file += ' '.join(str(nk) for nk in nk_list)
-            append_foot_file += "\n! reciprocal"
-        # Add kpoints    
-        for i, kp in enumerate(pc_kpoints_list):
-            append_foot_file += '\n!'
-            if kp is None:
-                append_foot_file += ' '
-            else:
-                append_foot_file += ' '.join(str(f'{kppp:12.8f}') for kppp in kp)
-                if labels is not None: append_foot_file += f'   {labels[i]}'
-        return append_foot_file
-    
-    def _generate_header_text(self, save_all_kpts:bool=False):
-        """
-        Create text that will be added in the front of file.
-
-        Parameters
-        ----------
-        save_all_kpts : bool, optional
-            Generate header text for the PC kpoints, generated SC kpoints, 
-            SC-PC kpoints mapping, and Special kpoints. 
-            The default is False. 
-
-        Returns
-        -------
-        header_msg : dictionary
-            Text string for header of save file. If save_all_kpts is True,
-            generate header text for the PC kpoints, generated SC kpoints, 
-            SC-PC kpoints mapping, and Special kpoints; else generate header
-            text only for SC kpoints.
-
-        """
-        # Generate header text for SC kpoints
-        header_msg = {}
-        header_msg['SC']  = f"K-points for SC bandstructure generated using banduppy-{__version__} package"
-        header_msg['SC'] += f"\n{len(self.SBZ_kpts_list)}\nreciprocal"
-        
-        header_msg['SpecialKpoints']   = f"Special SC kpoints indices generated using banduppy-{__version__} package"
-        header_msg['SpecialKpoints']  += "Kpoints index: Kpoints lebel"
-                
-        # Generate header text for PC kpoints, SC-PC kpoints mapping, and special kpoints  
-        if save_all_kpts:
-            # Create text that will be added in the front of file
-            header_msg['PC']  = f"k-points for PC bandstructure generated using banduppy-{__version__} package"
-            header_msg['PC'] += f"\n{len(self.PBZ_kpts_list_org)}\nreciprocal"
-            
-            header_msg['SCPC_map']  = f"Mapping for SC Kpoints to PC kpoints indices generated using banduppy-{__version__} package"
-            header_msg['SCPC_map'] += "K-k relation: (K index: K -> k index unique: k unique -> k index: k)"
-            
-        return header_msg
-    
-    def _generate_footer_text(self, footer_text=None, save_all_kpts:bool=False):
-        """
-        Create text that will be added in the bottom of file.
-
-        Parameters
-        ----------
-        footer_text: str, optional
-            Footer message. 
-        save_all_kpts : bool, optional
-            Generate footer text for the PC kpoints, generated SC kpoints, 
-            SC-PC kpoints mapping, and Special kpoints. 
-            The default is False. 
-
-        Returns
-        -------
-        footer_msg : dictionary
-            Text string for footer of save file. If save_all_kpts is True,
-            generate footer text for the PC kpoints, generated SC kpoints, 
-            SC-PC kpoints mapping, and Special kpoints; else generate footer
-            text only for SC kpoints.
-
-        """
-        # Generate footer text for SC kpoints
-        footer_msg = {}
-        footer_msg['SC'] = self._generate_foot_text(self.PBZ_kpts_list_org) if footer_text is None else footer_text
-        footer_msg['SpecialKpoints'] = ''
-        
-        # Save PC, SC kpoints    
-        if save_all_kpts:
-            footer_msg['PC'] = footer_msg['SC']
-            footer_msg['SCPC_map'] = ''
-        return footer_msg
-    
-    def _generate_print_text(self, save_all_kpts:bool=False):
-        """
-        Create text that will be printed when print information is True.
-
-        Parameters
-        ----------
-        save_all_kpts : bool, optional
-            Generate print message for the PC kpoints, generated SC kpoints, 
-            SC-PC kpoints mapping, and Special kpoints. 
-            The default is False. 
-
-        Returns
-        -------
-        print_msg : dictionary
-            Text string for print msg when saving to file. If save_all_kpts is True,
-            generate msg text for the PC kpoints, generated SC kpoints, 
-            SC-PC kpoints mapping, and Special kpoints; else generate msg
-            text only for SC kpoints.
-
-        """
-        # Generate footer text for SC kpoints
-        print_msg = {}
-        print_msg['SC'] = 'Saving Kpoints to file...'
-        print_msg['SpecialKpoints'] = 'Saving special kpoints position indices and labels to file...'
-            
-        # Save PC, SC kpoints    
-        if save_all_kpts:
-            print_msg['PC'] = 'Saving kpoints to file...'
-            print_msg['SCPC_map'] = 'Saving SC Kpoints - PC kpoints indices mapping to file...'           
-        return print_msg
-
-    def _generate_save_contents(self, footer_text=None, save_all_kpts:bool=False):
-        """
-        Create (kpoints) data that will be saved to file.
-
-        Parameters
-        ----------
-        footer_text: str, optional
-            Footer message. 
-        save_all_kpts : bool, optional
-            Generate data for the PC kpoints, generated SC kpoints, 
-            SC-PC kpoints mapping, and Special kpoints. 
-            The default is False. 
-
-        Returns
-        -------
-        save_contents_data : dictionary
-            Header, footer texts and data to be saved. If save_all_kpts is True,
-            generate data for the PC kpoints, generated SC kpoints, 
-            SC-PC kpoints mapping, and Special kpoints; else generate data
-            only for SC kpoints.
-
-        """
-        save_contents_data = {}
-        header_msg_ = self._generate_header_text(save_all_kpts=save_all_kpts)
-        footer_msg_ = self._generate_footer_text(footer_text=footer_text, save_all_kpts=save_all_kpts)
-        print_msg_ = self._generate_print_text(save_all_kpts=save_all_kpts)
-
-        save_contents_data['SC'] = (header_msg_['SC'], self.SBZ_kpts_list, 
-                                    footer_msg_['SC'], print_msg_['SC'])  
-        save_contents_data['SpecialKpoints'] = (header_msg_['SpecialKpoints'], 
-                                                self.special_kpoints_pos_labels, 
-                                                footer_msg_['SpecialKpoints'],
-                                                print_msg_['SpecialKpoints'])
-        if save_all_kpts:
-            save_contents_data['PC'] = (header_msg_['PC'], 
-                                        self.PBZ_kpts_list_org, 
-                                        footer_msg_['PC'],
-                                        print_msg_['PC'])
-            save_contents_data['SCPC_map'] = (header_msg_['SCPC_map'], 
-                                              self.SBZ_PBZ_kpts_mapping, 
-                                              footer_msg_['SCPC_map'],
-                                              print_msg_['SCPC_map'])
-        return save_contents_data
-
-## ============================================================================ 
-class BandFolding(_KpointsModule, FindProperties):
-    """
-    Band folding from primitive to supercell.
-
-    """
-    def __init__(self, supercell=None, print_info='low'):
-        """
-        Initialize the Folding class.
-
-        Parameters
-        ----------
-        supercell : 3X3 matrix, optional
-            Primitive-to-supercell transformation matrix. The default is Identity matrix.
-        print_info : [None,'low','medium','high'], optional
-            Print information of kpoints folding. Level of printing information. 
-            The default is 'low'. If None, nothing is printed.
-
-        """
-        if supercell is None: supercell = np.eye(3,dtype=int)
-        self.transformation_matrix = _BasicFunctionsModule._check_transformation_matrix(np.array(supercell)) 
-        self.print_information = print_info
-                   
-    def propose_best_least_folding(self, pathPBZ, min_num_pts:int=5, max_num_pts:int=20,
-                                   serach_mode:str='brute_force'):
-        """
-        Calculates SC Kpoints from PC kpoints and returns percent of folding.
-        Maximum and Minimum degree of folding are reported.
-        
-        Folding percent = (#of PC kpoints - #of folded SC Kpoints)/(#of PC kpoints))*100
-
-        Parameters
-        ----------
-        pathPBZ : ndarray/list
-            PC kpoint path nodes in reduced coordinates.
-        min_num_pts : int, optional
-            Minimum number of kpoints division in the k-path. The default is 5.
-        max_num_pts : int, optional
-            Maximum number of kpoints division in the k-path. The default is 20.
-        serach_mode : ['brute_force'], optional
-            Method to calculate SC Kpoints. The default is 'brute_force'.
-
-        Returns
-        -------
-        proposed_folding_results : dictionary
-            {index: ((start node, end node), folding data)}
-            index : Index of path segment searched from the pathPBZ list supplied.
-            folding data : 2d array with each row containing number of division in the 1st
-            column and percent of folding in the 2nd column.
-            
-        """
-        return self._propose_max_min_folding(self.transformation_matrix, pathPBZ, 
-                                             min_num_pts=min_num_pts, 
-                                             max_num_pts=max_num_pts,
-                                             serach_mode=serach_mode)
-    
-    def generate_SC_K_from_pc_k_path(self, pathPBZ=None, nk=11, labels=None, kpts_weights=None, 
-                                     save_all_kpts:bool=False, save_sc_kpts:bool=False, 
-                                     save_dir='.', file_name:str='', 
-                                     file_name_suffix:str='', file_format:str='vasp'):
-        """
-        Generate supercell kpoints from reference primitive BZ k-path.
-
-        Parameters
-        ----------
-        pathPBZ : ndarray/list, optional
-            PC kpoint path nodes in reduced coordinates. 
-            If the segmant is skipped, put a None between nodes.
-            E.g. [[1/2,1/2,1/2], [0,0,0],None, [3/8,3/8,3/4], [0,0,0]] for [LGKG]
-            The default is None. 
-        nk : int ot tuple, optional
-            Number of kpoints in each k-path segment. The default is 11.
-            None in pathPBZ is not part of the segments. 
-            E.g. In [[1/2,1/2,1/2], [0,0,0],None, [3/8,3/8,3/4], [0,0,0]] there are
-            only 2 segments.
-        labels : string ot list of strings
-            Labels of special k-points, either as a continuous list or string. 
-            Do not use ',' or multidimentional list do define disjoint segmants.
-            e.g. Do not use labels='LG,KG'. Use labels='LGKG'. The 'None' in the
-            pathPBZ will take care of the disjoint segments.
-            If multiple word needs to be single label, use list.
-            e.g. labels=['X','Gamma','L']. Do not use string labels='XGammaL'.
-            The default is None. If None, the special
-            kpoints will be indexed as 1,2,3,...
-        kpts_weights : int or float or 1d numpy array, optional
-            Weights of the SC kpoints. The default is None. If none, no weights are padded
-            in the generated SC K-points list.
-        save_all_kpts : bool, optional
-            Save the PC kpoints, generated SC kpoints, and SC-PC kpoints mapping. 
-            The default is False. If True, has precedence over save_sc_kpts.
-        save_sc_kpts : bool, optional
-            Save the generated SC kpoints. The default is False.
-        save_dir : str/path_object, optional
-            Directory to save the file. The default is current directory.
-        file_name : str, optional
-            Name of the file. The default is ''.
-            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
-        file_name_suffix : str, optional
-            Suffix to add after the file_name. The default is ''.
-        file_format : ['vasp'], optional
-            Format of the file. The default is 'vasp'. 
-            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
-
-        Returns
-        -------
-        ndarray of floats
-            PC kpoints list.
-        ndarray of floats
-            SC kpoints list.
-        ndarray of int
-            PC unique kpoints indices for reverse engineer.
-        ndarray of int
-            SC unique kpoints indices for reverse engineer.
-
-        """
-        assert pathPBZ is not None, 'pathPBZ should not be None.'
-        
-        # Create PC kpoints from k-path
-        PBZ_kpts, special_kpoints_pos_labels, nkgen, labels  = self._generate_kpts_from_kpath(pathPBZ, nk, labels)
-        
-        # Save SC kpoints
-        footer_msg_path = None
-        if save_sc_kpts:
-            footer_msg_path = self._generate_foot_text(pathPBZ, labels=labels, nk_list=nk)
- 
-        # Return SC kpoints from PC k-path k-points        
-        return self.generate_K_from_k(kpointsPBZ=PBZ_kpts, kpts_weights=kpts_weights, 
-                                      save_all_kpts=save_all_kpts,
-                                      save_sc_kpts=save_sc_kpts, save_dir=save_dir, 
-                                      file_name=file_name, file_name_suffix=file_name_suffix, 
-                                      file_format=file_format, footer_msg=footer_msg_path,
-                                      special_kpoints_pos_labels=special_kpoints_pos_labels) 
-            
-    def generate_K_from_k(self, kpointsPBZ=None, kpts_weights=None,
-                          save_all_kpts:bool=False, save_sc_kpts:bool=False, 
-                          save_dir='.', file_name:str='', 
-                          file_name_suffix:str='', file_format:str='vasp', footer_msg=None,
-                          special_kpoints_pos_labels=None):
-        """
-        Generate supercell kpoints from reference primitive kpoints.
-
-        Parameters
-        ----------
-        kpointsPBZ : ndarray, optional
-            PC kpoint list. The default is None. 
-        kpts_weights : int or float or 1d numpy array, optional
-            Weights of the SC kpoints. The default is None. If none, no weights are padded
-            in the generated SC K-points list.
-        save_all_kpts : bool, optional
-            Save the PC kpoints, generated SC kpoints, and SC-PC kpoints mapping. 
-            The default is False. If True, has precedence over save_sc_kpts.
-        save_sc_kpts : bool, optional
-            Save the generated SC kpoints. The default is False.
-        save_dir : str/path_object, optional
-            Directory to save the file. The default is current directory.
-        file_name : str, optional
-            Name of the file. The default is ''.
-            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
-        file_name_suffix : str, optional
-            Suffix to add after the file_name. The default is ''.
-        file_format : ['vasp'], optional
-            Format of the file. The default is 'vasp'. 
-            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
-        footer_msg : str, optional
-            String that will be written at the end of the file. The default is PC kpoints list.
-        special_kpoints_pos_labels : dictionary, optional
-            Special kpoints position_index in PC kpoints list as key and label as value. 
-            Will be used in plotting. Default is None.
-
-        Returns
-        -------
-        ndarray of floats
-            PC kpoints list (orginal provided k-path, full list).
-        ndarray of floats
-            PC kpoints list (unique).
-        ndarray of floats
-            SC kpoints list (unique).
-        dictionary of int/list
-            Mapping of SC kpts (K), PC unique kpts (k unique), and PC full kpts (k) indices.
-            format: {K index: K -> k index unique: k unique -> k index: k}
-            This mapping can be used for reverse engineer latter.
-        dictionary or None
-            Position and labels of special kpoints, will be used in plotting.
-
-        """
-        assert kpointsPBZ is not None, 'kpointsPBZ should not be None.'
-        
-        # Original PC kpoints list
-        self.PBZ_kpts_list_org = np.copy(kpointsPBZ)
-        # Generate SC kpoints list
-        self.PBZ_kpts_list, self.kpointsPBZ_index_in_unique = self._remove_duplicate_kpoints(self.PBZ_kpts_list_org)
-        kpointsSBZ = self._find_K_from_k(self.PBZ_kpts_list, self.transformation_matrix)
-        self.SBZ_kpts_list, self.kpointsSBZ_index_in_unique = self._remove_duplicate_kpoints(kpointsSBZ)
-        self._get_PBZ_SBZ_kpts_mapping()
-        
-        # Pad the kpoints weights if exists
-        if kpts_weights is not None:
-            self.SBZ_kpts_list = self._pad_kpts_weights(self.SBZ_kpts_list, kpts_weights=kpts_weights)
-        
-        # Special kpoints
-        self.special_kpoints_pos_labels = special_kpoints_pos_labels
-        
-        # Print information about folding
-        if self.print_information is not None: 
-            self._print_info(level=self.print_information)
-            
-        # Saving kpoints data
-        if save_all_kpts or save_sc_kpts:
-            # save_contents_data: (header text, data, footer text, print message)
-            save_contents_data = self. _generate_save_contents(footer_text=footer_msg, 
-                                                               save_all_kpts=save_all_kpts)
-            for data_key, data_items in save_contents_data.items():
-                SaveData2File.save_sc_kpts_2_file(data=data_items[1],
-                                                  save_dir=save_dir, file_name=file_name,
-                                                  file_name_suffix=f'{file_name_suffix}_{data_key}', 
-                                                  file_format=file_format,
-                                                  header_txt=data_items[0], 
-                                                  footer_txt=data_items[2],
-                                                  print_log=bool(self.print_information),
-                                                  print_msg=data_items[3])
-        
-        return self.PBZ_kpts_list_org, self.PBZ_kpts_list, self.SBZ_kpts_list, \
-                self.SBZ_PBZ_kpts_mapping, self.special_kpoints_pos_labels
-
+import numpy as np
+from ..BasicFunctions.general_functions import SaveData2File, _BasicFunctionsModule, _draw_line_length
+from .folding_properties import FindProperties
+from .. import __version__
+    
+try:
+    from collections.abc import Iterable
+except ImportError:
+    from collections import Iterable
+    
+## ============================================================================    
+class _KpointsModule:   
+    
+    @staticmethod
+    def _find_K_from_k(k, transformation_matrix):
+        """
+        Generate list of SC K-vectors onto which the PC k-vectors folds. 
+        
+            K = k.P
+
+        Parameters
+        ----------
+        k : ndarray of floats
+            PC kpoints.
+        transformation_matrix : ndarray
+            PC to SC transformation matrix.
+
+        Returns
+        -------
+        ndarray of floats
+            SC kpoints.
+
+        """
+        return np.dot(k, transformation_matrix.T)
+
+    @classmethod   
+    def _remove_duplicate_kpoints(cls, kpoints, sort_kpts:bool=False, 
+                                  return_id_mapping:bool=True, decimals:int=10):
+        """
+        Remove duplicate kpoints.
+
+        Parameters
+        ----------
+        kpoints : ndarray of floats
+            kpoints list.
+        sort_kpts : bool, optional
+            Sort the kpoints. The default is False.
+        return_id_mapping : bool, optional
+            Return the id of reverse mapping. The default is True.
+        decimals : int, optional
+            How many decomal points to round up. The default is 10.
+
+        Returns
+        -------
+        ndarray of floats, ndarray of int
+            Reduced kpoint list.
+
+        """
+        kpoints = np.asarray(kpoints)
+        unique_kpts, unique_kpts_ids, kpts_ids = np.unique(_BasicFunctionsModule._return_mod(kpoints),
+                                                           axis=0, return_index=True, return_inverse=True)
+        
+        if sort_kpts:
+            sort_pos_kpts = np.argsort(unique_kpts_ids)
+            unique_kpts_ids = unique_kpts_ids[sort_pos_kpts]
+            unique_kpts = kpoints[unique_kpts_ids]
+            kpts_ids = kpts_ids[sort_pos_kpts]
+
+        if return_id_mapping:
+            return unique_kpts, kpts_ids
+        else:
+            return unique_kpts
+    
+    @classmethod
+    def _search_folding_percent_brute_force(cls, transformation_matrix, start, end, 
+                                            min_div_points, max_div_points):  
+        """
+        Calculates SC Kpoints from PC kpoints and returns percent of folding.
+        This method uses brute force to calculate folding degree i.e. complete
+        list of SC Kpoints are generated in the process. 
+        (Loop over nkpoints in the path segment starting with min_div_points until
+        max_div_points with increment of 1.)
+        
+        Folding percent = ((#of PC kpoints - #of folded SC Kpoints)/(#of PC kpoints))*100
+
+        Parameters
+        ----------
+        transformation_matrix : ndarray
+            PC to SC transformation matrix.
+        start : 1d array
+            Starting coordinate of kpoints path.
+        end : 1d array
+            End coordinate of kpoints path.
+        min_div_points : int
+            Minimum number of kpoints division in the k-path.
+        max_div_points : int
+            Maximum number of kpoints division in the k-path.
+
+        Returns
+        -------
+        numpy ndarray
+            2d array with each row containing number of division in the 1st
+            column and percent of folding in the 2nd column.
+
+        """
+        folding_info_list = []
+        # Loop over nkpoints in the path segment starting with min_div_points until
+        # max_div_points with increment of 1.
+        for div_points in range(min_div_points, max_div_points): 
+            len_unique_Kpts = \
+            len(cls._remove_duplicate_kpoints(
+                _KpointsModule._find_K_from_k(np.linspace(start, end, div_points), 
+                                                            transformation_matrix),
+                sort_kpts=False, return_id_mapping=False))
+            
+            folding_info_list.append([div_points, 
+                                      (div_points-len_unique_Kpts)/div_points*100]) 
+        return np.array(folding_info_list)
+
+    @classmethod           
+    def _serach_max_min_folding(cls, transformation_matrix, start, end, 
+                                min_num_pts:int=5, max_num_pts:int=20,
+                                serach_mode:str='brute_force'):
+        """
+        Calculates SC Kpoints from PC kpoints and returns percent of folding.
+        Maximum and Minimum degree of folding are reported.
+        
+        Folding percent = ((#of PC kpoints - #of folded SC Kpoints)/(#of PC kpoints))*100
+
+        Parameters
+        ----------
+        transformation_matrix : ndarray
+            PC to SC transformation matrix.
+        start : 1d array
+            Starting coordinate of kpoints path.
+        end : 1d array
+            End coordinate of kpoints path.
+        min_num_pts : int, optional
+            Minimum number of kpoints division in the k-path. The default is 5.
+        max_num_pts : int, optional
+            Maximum number of kpoints division in the k-path. The default is 20.
+        serach_mode : ['brute_force'], optional
+            Method to calculate SC Kpoints. The default is 'brute_force'.
+
+        Returns
+        -------
+        folding_data_ : numpy ndarray
+            2d array with each row containing number of division in the 1st
+            column and percent of folding in the 2nd column.
+
+        """
+        assert max_num_pts >= min_num_pts, f'max_num_pts should be >= min_num_pts {min_num_pts}.'
+        if serach_mode == 'brute_force':
+            folding_data_ = cls._search_folding_percent_brute_force(transformation_matrix, 
+                                                                    start, end, 
+                                                                    min_num_pts, max_num_pts)
+            max_folding = folding_data_[np.argmax(folding_data_[:,1])]
+            min_folding = folding_data_[np.argmin(folding_data_[:,1])]
+            print(f'--- Maximum folding (nkpts, folding percent): {int(max_folding[0]):>3d}, {max_folding[1]:.3f}%')
+            print(f'--- Minimum folding (nkpts, folding percent): {int(min_folding[0]):>3d}, {min_folding[1]:.3f}%')
+            return folding_data_ 
+        
+    @classmethod           
+    def _propose_max_min_folding(cls, transformation_matrix, pathPBZ, 
+                                 min_num_pts:int=5, max_num_pts:int=20,
+                                 serach_mode:str='brute_force'):
+        """
+        Calculates SC Kpoints from PC kpoints and returns percent of folding.
+        Maximum and Minimum degree of folding are reported.
+        
+        Folding percent = ((#of PC kpoints - #of folded SC Kpoints)/(#of PC kpoints))*100
+
+        Parameters
+        ----------
+        transformation_matrix : ndarray
+            PC to SC transformation matrix.
+        pathPBZ : ndarray/list
+            PC kpoint path nodes in reduced coordinates.
+        min_num_pts : int, optional
+            Minimum number of kpoints division in the k-path. The default is 5.
+        max_num_pts : int, optional
+            Maximum number of kpoints division in the k-path. The default is 20.
+        serach_mode : ['brute_force'], optional
+            Method to calculate SC Kpoints. The default is 'brute_force'.
+
+        Returns
+        -------
+        propose_folding_data_ : dictionary
+            {index: ((start node, end node), folding data)}
+            index : Index of path segment searched from the pathPBZ list supplied.
+            folding data : 2d array with each row containing number of division in the 1st
+            column and percent of folding in the 2nd column.
+
+        """
+        propose_folding_data_ = {}
+        print(f"{'='*_draw_line_length}\n- Proposing maximum and minimum band folding...")
+        # Iterate over the list, skipping the last element
+        for i in range(len(pathPBZ) - 1):
+            # Check if both current and next elements are not None
+            if pathPBZ[i] is not None and pathPBZ[i + 1] is not None:
+                # Get start and end of k-path segment
+                start, end = np.array(pathPBZ[i]), np.array(pathPBZ[i + 1])
+                assert start.shape == end.shape == (3,)
+                print(f'-- k-path: {start} --> {end}')
+                # Search for max-min folding
+                propose_folding_data_[i] = ((start, end),
+                    cls._serach_max_min_folding(transformation_matrix, start, end, 
+                                                                       min_num_pts=min_num_pts, 
+                                                                       max_num_pts=max_num_pts,
+                                                                       serach_mode=serach_mode))
+        return propose_folding_data_
+
+        
+    @staticmethod   
+    def _generate_kpts_from_kpath(pathPBZ, nk, labels):
+        """
+        Creates
+
+        Parameters
+        ----------
+        pathPBZ : ndarray/list, optional
+            PC kpoint path nodes in reduced coordinates. 
+        nk : int ot tuple, optional
+            Number of kpoints in each k-path segment. 
+        labels : string ot list of strings
+            Labels of special k-points, either as a continuous list or string. 
+            Do not use ',' or multidimentional list do define disjoint segmants.
+            e.g. Do not use labels='LG,KG'. Use labels='LGKG'. The 'None' in the
+            pathPBZ will take care of the disjoint segments.
+            If multiple word needs to be single label, use list.
+            e.g. labels=['X','Gamma','L']. Do not use string labels='XGammaL'.
+            If None, the special kpoints will be indexed as 1,2,3,...
+
+        Returns
+        -------
+        kpointsPBZ : ndarray, optional
+            PC kpoint list. 
+        special_kpoints_pos_labels : dictionary
+            Special k-points position and labels.
+
+        """
+        # List of number_of_kpoints in segment
+        # Convert nk to generator if it's iterable
+        nkgen = (x for x in nk) if isinstance(nk, Iterable) else (nk for _ in pathPBZ)
+        
+        # Total nodes in the PC BZ supplied
+        total_k_nodes = len([1 for k in pathPBZ if k is not None])
+        
+        # Create labels list for special_kpoints_labels
+        if labels is None:
+            labels = [str(i+1) for i in range(total_k_nodes)]
+        else:
+            assert len(labels) >= total_k_nodes , 'Number of labels is less than the supplied k-path segments.'
+        labels = (l for l in labels)
+        labels = [None if k is None else next(labels) for k in pathPBZ]
+        
+        # Initialize
+        kpointsPBZ=np.zeros((0,3))
+        special_kpoints_pos_labels={}
+        
+        # Iterate over the list, skipping the last element
+        for i in range(len(pathPBZ) - 1):
+            # Check if both current and next elements are not None
+            if pathPBZ[i] is not None and pathPBZ[i + 1] is not None:
+                # Get position of special k-point for plotting later
+                special_kpoints_pos_labels[kpointsPBZ.shape[0]] = labels[i]
+                # Get start and end of k-path segment
+                start, end = np.array(pathPBZ[i]), np.array(pathPBZ[i + 1])
+                assert start.shape == end.shape == (3,)
+                # Get nk in k-path segment
+                try:
+                    num_points = next(nkgen)
+                except: 
+                    raise StopIteration('Number of nk is less than the supplied k-path segments.')
+                # Generate k-points using linspace
+                interpolated_points = np.linspace(start, end, num_points)
+                kpointsPBZ = np.vstack((kpointsPBZ, interpolated_points))
+                # Get position of special k-point for plotting later
+                special_kpoints_pos_labels[kpointsPBZ.shape[0] - 1] = labels[i+1] 
+    
+        return kpointsPBZ, special_kpoints_pos_labels, nkgen, labels
+    
+    @staticmethod
+    def _pad_kpts_weights(kpoints, kpts_weights=1):
+        """
+        Padding the weights of SC kpoints.
+
+        Parameters
+        ----------
+        kpoints : ndarray of floats
+            kpoints list.
+        kpts_weights : int or float or 1d numpy array, optional
+            Weights of the SC kpoints. The default is 1.
+
+        Returns
+        -------
+        ndarray of floats
+            kpoints list padded with weights.
+
+        """
+
+        if isinstance(kpts_weights, int) or isinstance(kpts_weights, float):
+            append_weights = np.array([[kpts_weights]*len(kpoints)])
+        else:
+            append_weights = np.copy([kpts_weights])
+        return np.concatenate((kpoints, append_weights.T), axis=1)
+    
+    @staticmethod
+    def _generate_foot_text(pc_kpoints_list, labels=None, nk_list=None):
+        """
+        Create foorter text for the SC kpoints save file.
+
+        Parameters
+        ----------
+        pc_kpoints_list : ndarray/list
+            List of PC kpoints or k-path.
+        labels : list, optional
+            List of special k-points in k-path. The default is None.
+        nk_list : list, optional
+            List of number of k-points in each k-path segments. The default is None.
+
+        Returns
+        -------
+        append_foot_file : str
+            Text string for footer of save file.
+
+        """
+        append_foot_file  = '\n\n! The above SCKPTS (and/or some other SCKPTS related to them by symm. ops. of the SCBZ)'
+        append_foot_file += '\n! unfold onto the pckpts listed below (selected by you):'
+        append_foot_file += '\n! k-points for PC bandstructure '
+        # Add label texts
+        if labels is not None:                   
+            append_foot_file += ','.join('-'.join(label for label in group_ if label) 
+                                         for group_ in ''.join(str(label) for label in labels).split('None') if group_)         
+        # Add number of kpoints in each segment
+        if nk_list is not None: 
+            if not isinstance(nk_list, Iterable): nk_list = [nk_list]
+            append_foot_file += '\n! '
+            append_foot_file += ' '.join(str(nk) for nk in nk_list)
+            append_foot_file += "\n! reciprocal"
+        # Add kpoints    
+        for i, kp in enumerate(pc_kpoints_list):
+            append_foot_file += '\n!'
+            if kp is None:
+                append_foot_file += ' '
+            else:
+                append_foot_file += ' '.join(str(f'{kppp:12.8f}') for kppp in kp)
+                if labels is not None: append_foot_file += f'   {labels[i]}'
+        return append_foot_file
+    
+    def _generate_header_text(self, save_all_kpts:bool=False):
+        """
+        Create text that will be added in the front of file.
+
+        Parameters
+        ----------
+        save_all_kpts : bool, optional
+            Generate header text for the PC kpoints, generated SC kpoints, 
+            SC-PC kpoints mapping, and Special kpoints. 
+            The default is False. 
+
+        Returns
+        -------
+        header_msg : dictionary
+            Text string for header of save file. If save_all_kpts is True,
+            generate header text for the PC kpoints, generated SC kpoints, 
+            SC-PC kpoints mapping, and Special kpoints; else generate header
+            text only for SC kpoints.
+
+        """
+        # Generate header text for SC kpoints
+        header_msg = {}
+        header_msg['SC']  = f"K-points for SC bandstructure generated using banduppy-{__version__} package"
+        header_msg['SC'] += f"\n{len(self.SBZ_kpts_list)}\nreciprocal"
+        
+        header_msg['SpecialKpoints']   = f"Special SC kpoints indices generated using banduppy-{__version__} package"
+        header_msg['SpecialKpoints']  += "Kpoints index: Kpoints lebel"
+                
+        # Generate header text for PC kpoints, SC-PC kpoints mapping, and special kpoints  
+        if save_all_kpts:
+            # Create text that will be added in the front of file
+            header_msg['PC']  = f"k-points for PC bandstructure generated using banduppy-{__version__} package"
+            header_msg['PC'] += f"\n{len(self.PBZ_kpts_list_org)}\nreciprocal"
+            
+            header_msg['SCPC_map']  = f"Mapping for SC Kpoints to PC kpoints indices generated using banduppy-{__version__} package"
+            header_msg['SCPC_map'] += "K-k relation: (K index: K -> k index unique: k unique -> k index: k)"
+            
+        return header_msg
+    
+    def _generate_footer_text(self, footer_text=None, save_all_kpts:bool=False):
+        """
+        Create text that will be added in the bottom of file.
+
+        Parameters
+        ----------
+        footer_text: str, optional
+            Footer message. 
+        save_all_kpts : bool, optional
+            Generate footer text for the PC kpoints, generated SC kpoints, 
+            SC-PC kpoints mapping, and Special kpoints. 
+            The default is False. 
+
+        Returns
+        -------
+        footer_msg : dictionary
+            Text string for footer of save file. If save_all_kpts is True,
+            generate footer text for the PC kpoints, generated SC kpoints, 
+            SC-PC kpoints mapping, and Special kpoints; else generate footer
+            text only for SC kpoints.
+
+        """
+        # Generate footer text for SC kpoints
+        footer_msg = {}
+        footer_msg['SC'] = self._generate_foot_text(self.PBZ_kpts_list_org) if footer_text is None else footer_text
+        footer_msg['SpecialKpoints'] = ''
+        
+        # Save PC, SC kpoints    
+        if save_all_kpts:
+            footer_msg['PC'] = footer_msg['SC']
+            footer_msg['SCPC_map'] = ''
+        return footer_msg
+    
+    def _generate_print_text(self, save_all_kpts:bool=False):
+        """
+        Create text that will be printed when print information is True.
+
+        Parameters
+        ----------
+        save_all_kpts : bool, optional
+            Generate print message for the PC kpoints, generated SC kpoints, 
+            SC-PC kpoints mapping, and Special kpoints. 
+            The default is False. 
+
+        Returns
+        -------
+        print_msg : dictionary
+            Text string for print msg when saving to file. If save_all_kpts is True,
+            generate msg text for the PC kpoints, generated SC kpoints, 
+            SC-PC kpoints mapping, and Special kpoints; else generate msg
+            text only for SC kpoints.
+
+        """
+        # Generate footer text for SC kpoints
+        print_msg = {}
+        print_msg['SC'] = 'Saving Kpoints to file...'
+        print_msg['SpecialKpoints'] = 'Saving special kpoints position indices and labels to file...'
+            
+        # Save PC, SC kpoints    
+        if save_all_kpts:
+            print_msg['PC'] = 'Saving kpoints to file...'
+            print_msg['SCPC_map'] = 'Saving SC Kpoints - PC kpoints indices mapping to file...'           
+        return print_msg
+
+    def _generate_save_contents(self, footer_text=None, save_all_kpts:bool=False):
+        """
+        Create (kpoints) data that will be saved to file.
+
+        Parameters
+        ----------
+        footer_text: str, optional
+            Footer message. 
+        save_all_kpts : bool, optional
+            Generate data for the PC kpoints, generated SC kpoints, 
+            SC-PC kpoints mapping, and Special kpoints. 
+            The default is False. 
+
+        Returns
+        -------
+        save_contents_data : dictionary
+            Header, footer texts and data to be saved. If save_all_kpts is True,
+            generate data for the PC kpoints, generated SC kpoints, 
+            SC-PC kpoints mapping, and Special kpoints; else generate data
+            only for SC kpoints.
+
+        """
+        save_contents_data = {}
+        header_msg_ = self._generate_header_text(save_all_kpts=save_all_kpts)
+        footer_msg_ = self._generate_footer_text(footer_text=footer_text, save_all_kpts=save_all_kpts)
+        print_msg_ = self._generate_print_text(save_all_kpts=save_all_kpts)
+
+        save_contents_data['SC'] = (header_msg_['SC'], self.SBZ_kpts_list, 
+                                    footer_msg_['SC'], print_msg_['SC'])  
+        save_contents_data['SpecialKpoints'] = (header_msg_['SpecialKpoints'], 
+                                                self.special_kpoints_pos_labels, 
+                                                footer_msg_['SpecialKpoints'],
+                                                print_msg_['SpecialKpoints'])
+        if save_all_kpts:
+            save_contents_data['PC'] = (header_msg_['PC'], 
+                                        self.PBZ_kpts_list_org, 
+                                        footer_msg_['PC'],
+                                        print_msg_['PC'])
+            save_contents_data['SCPC_map'] = (header_msg_['SCPC_map'], 
+                                              self.SBZ_PBZ_kpts_mapping, 
+                                              footer_msg_['SCPC_map'],
+                                              print_msg_['SCPC_map'])
+        return save_contents_data
+
+## ============================================================================ 
+class BandFolding(_KpointsModule, FindProperties):
+    """
+    Band folding from primitive to supercell.
+
+    """
+    def __init__(self, supercell=None, print_info='low'):
+        """
+        Initialize the Folding class.
+
+        Parameters
+        ----------
+        supercell : 3X3 matrix, optional
+            Primitive-to-supercell transformation matrix. The default is Identity matrix.
+        print_info : [None,'low','medium','high'], optional
+            Print information of kpoints folding. Level of printing information. 
+            The default is 'low'. If None, nothing is printed.
+
+        """
+        if supercell is None: supercell = np.eye(3,dtype=int)
+        self.transformation_matrix = _BasicFunctionsModule._check_transformation_matrix(np.array(supercell)) 
+        self.print_information = print_info
+                   
+    def propose_best_least_folding(self, pathPBZ, min_num_pts:int=5, max_num_pts:int=20,
+                                   serach_mode:str='brute_force'):
+        """
+        Calculates SC Kpoints from PC kpoints and returns percent of folding.
+        Maximum and Minimum degree of folding are reported.
+        
+        Folding percent = (#of PC kpoints - #of folded SC Kpoints)/(#of PC kpoints))*100
+
+        Parameters
+        ----------
+        pathPBZ : ndarray/list
+            PC kpoint path nodes in reduced coordinates.
+        min_num_pts : int, optional
+            Minimum number of kpoints division in the k-path. The default is 5.
+        max_num_pts : int, optional
+            Maximum number of kpoints division in the k-path. The default is 20.
+        serach_mode : ['brute_force'], optional
+            Method to calculate SC Kpoints. The default is 'brute_force'.
+
+        Returns
+        -------
+        proposed_folding_results : dictionary
+            {index: ((start node, end node), folding data)}
+            index : Index of path segment searched from the pathPBZ list supplied.
+            folding data : 2d array with each row containing number of division in the 1st
+            column and percent of folding in the 2nd column.
+            
+        """
+        return self._propose_max_min_folding(self.transformation_matrix, pathPBZ, 
+                                             min_num_pts=min_num_pts, 
+                                             max_num_pts=max_num_pts,
+                                             serach_mode=serach_mode)
+    
+    def generate_SC_K_from_pc_k_path(self, pathPBZ=None, nk=11, labels=None, kpts_weights=None, 
+                                     save_all_kpts:bool=False, save_sc_kpts:bool=False, 
+                                     save_dir='.', file_name:str='', 
+                                     file_name_suffix:str='', file_format:str='vasp'):
+        """
+        Generate supercell kpoints from reference primitive BZ k-path.
+
+        Parameters
+        ----------
+        pathPBZ : ndarray/list, optional
+            PC kpoint path nodes in reduced coordinates. 
+            If the segmant is skipped, put a None between nodes.
+            E.g. [[1/2,1/2,1/2], [0,0,0],None, [3/8,3/8,3/4], [0,0,0]] for [LGKG]
+            The default is None. 
+        nk : int ot tuple, optional
+            Number of kpoints in each k-path segment. The default is 11.
+            None in pathPBZ is not part of the segments. 
+            E.g. In [[1/2,1/2,1/2], [0,0,0],None, [3/8,3/8,3/4], [0,0,0]] there are
+            only 2 segments.
+        labels : string ot list of strings
+            Labels of special k-points, either as a continuous list or string. 
+            Do not use ',' or multidimentional list do define disjoint segmants.
+            e.g. Do not use labels='LG,KG'. Use labels='LGKG'. The 'None' in the
+            pathPBZ will take care of the disjoint segments.
+            If multiple word needs to be single label, use list.
+            e.g. labels=['X','Gamma','L']. Do not use string labels='XGammaL'.
+            The default is None. If None, the special
+            kpoints will be indexed as 1,2,3,...
+        kpts_weights : int or float or 1d numpy array, optional
+            Weights of the SC kpoints. The default is None. If none, no weights are padded
+            in the generated SC K-points list.
+        save_all_kpts : bool, optional
+            Save the PC kpoints, generated SC kpoints, and SC-PC kpoints mapping. 
+            The default is False. If True, has precedence over save_sc_kpts.
+        save_sc_kpts : bool, optional
+            Save the generated SC kpoints. The default is False.
+        save_dir : str/path_object, optional
+            Directory to save the file. The default is current directory.
+        file_name : str, optional
+            Name of the file. The default is ''.
+            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
+        file_name_suffix : str, optional
+            Suffix to add after the file_name. The default is ''.
+        file_format : ['vasp'], optional
+            Format of the file. The default is 'vasp'. 
+            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
+
+        Returns
+        -------
+        ndarray of floats
+            PC kpoints list.
+        ndarray of floats
+            SC kpoints list.
+        ndarray of int
+            PC unique kpoints indices for reverse engineer.
+        ndarray of int
+            SC unique kpoints indices for reverse engineer.
+
+        """
+        assert pathPBZ is not None, 'pathPBZ should not be None.'
+        
+        # Create PC kpoints from k-path
+        PBZ_kpts, special_kpoints_pos_labels, nkgen, labels  = self._generate_kpts_from_kpath(pathPBZ, nk, labels)
+        
+        # Save SC kpoints
+        footer_msg_path = None
+        if save_sc_kpts:
+            footer_msg_path = self._generate_foot_text(pathPBZ, labels=labels, nk_list=nk)
+ 
+        # Return SC kpoints from PC k-path k-points        
+        return self.generate_K_from_k(kpointsPBZ=PBZ_kpts, kpts_weights=kpts_weights, 
+                                      save_all_kpts=save_all_kpts,
+                                      save_sc_kpts=save_sc_kpts, save_dir=save_dir, 
+                                      file_name=file_name, file_name_suffix=file_name_suffix, 
+                                      file_format=file_format, footer_msg=footer_msg_path,
+                                      special_kpoints_pos_labels=special_kpoints_pos_labels) 
+            
+    def generate_K_from_k(self, kpointsPBZ=None, kpts_weights=None,
+                          save_all_kpts:bool=False, save_sc_kpts:bool=False, 
+                          save_dir='.', file_name:str='', 
+                          file_name_suffix:str='', file_format:str='vasp', footer_msg=None,
+                          special_kpoints_pos_labels=None):
+        """
+        Generate supercell kpoints from reference primitive kpoints.
+
+        Parameters
+        ----------
+        kpointsPBZ : ndarray, optional
+            PC kpoint list. The default is None. 
+        kpts_weights : int or float or 1d numpy array, optional
+            Weights of the SC kpoints. The default is None. If none, no weights are padded
+            in the generated SC K-points list.
+        save_all_kpts : bool, optional
+            Save the PC kpoints, generated SC kpoints, and SC-PC kpoints mapping. 
+            The default is False. If True, has precedence over save_sc_kpts.
+        save_sc_kpts : bool, optional
+            Save the generated SC kpoints. The default is False.
+        save_dir : str/path_object, optional
+            Directory to save the file. The default is current directory.
+        file_name : str, optional
+            Name of the file. The default is ''.
+            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
+        file_name_suffix : str, optional
+            Suffix to add after the file_name. The default is ''.
+        file_format : ['vasp'], optional
+            Format of the file. The default is 'vasp'. 
+            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
+        footer_msg : str, optional
+            String that will be written at the end of the file. The default is PC kpoints list.
+        special_kpoints_pos_labels : dictionary, optional
+            Special kpoints position_index in PC kpoints list as key and label as value. 
+            Will be used in plotting. Default is None.
+
+        Returns
+        -------
+        ndarray of floats
+            PC kpoints list (orginal provided k-path, full list).
+        ndarray of floats
+            PC kpoints list (unique).
+        ndarray of floats
+            SC kpoints list (unique).
+        dictionary of int/list
+            Mapping of SC kpts (K), PC unique kpts (k unique), and PC full kpts (k) indices.
+            format: {K index: K -> k index unique: k unique -> k index: k}
+            This mapping can be used for reverse engineer latter.
+        dictionary or None
+            Position and labels of special kpoints, will be used in plotting.
+
+        """
+        assert kpointsPBZ is not None, 'kpointsPBZ should not be None.'
+        
+        # Original PC kpoints list
+        self.PBZ_kpts_list_org = np.copy(kpointsPBZ)
+        # Generate SC kpoints list
+        self.PBZ_kpts_list, self.kpointsPBZ_index_in_unique = self._remove_duplicate_kpoints(self.PBZ_kpts_list_org)
+        kpointsSBZ = self._find_K_from_k(self.PBZ_kpts_list, self.transformation_matrix)
+        self.SBZ_kpts_list, self.kpointsSBZ_index_in_unique = self._remove_duplicate_kpoints(kpointsSBZ)
+        self._get_PBZ_SBZ_kpts_mapping()
+        
+        # Pad the kpoints weights if exists
+        if kpts_weights is not None:
+            self.SBZ_kpts_list = self._pad_kpts_weights(self.SBZ_kpts_list, kpts_weights=kpts_weights)
+        
+        # Special kpoints
+        self.special_kpoints_pos_labels = special_kpoints_pos_labels
+        
+        # Print information about folding
+        if self.print_information is not None: 
+            self._print_info(level=self.print_information)
+            
+        # Saving kpoints data
+        if save_all_kpts or save_sc_kpts:
+            # save_contents_data: (header text, data, footer text, print message)
+            save_contents_data = self. _generate_save_contents(footer_text=footer_msg, 
+                                                               save_all_kpts=save_all_kpts)
+            for data_key, data_items in save_contents_data.items():
+                SaveData2File.save_sc_kpts_2_file(data=data_items[1],
+                                                  save_dir=save_dir, file_name=file_name,
+                                                  file_name_suffix=f'{file_name_suffix}_{data_key}', 
+                                                  file_format=file_format,
+                                                  header_txt=data_items[0], 
+                                                  footer_txt=data_items[2],
+                                                  print_log=bool(self.print_information),
+                                                  print_msg=data_items[3])
+        
+        return self.PBZ_kpts_list_org, self.PBZ_kpts_list, self.SBZ_kpts_list, \
+                self.SBZ_PBZ_kpts_mapping, self.special_kpoints_pos_labels
+
```

### Comparing `banduppy-0.3.0/banduppy/src/folding_properties.py` & `banduppy-0.3.1/banduppy/src/folding_properties.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-import numpy as np
-from ..BasicFunctions.general_functions import _draw_line_length
-    
-### ===========================================================================
-class FindProperties:
-    def __init__(self):
-        pass
-    
-    @property
-    def nkptSBZ(self):
-        '''
-        Return number of (unique) SC kpoints.
-        '''
-        return(self.SBZ_kpts_list.shape[0])
-    
-    @property
-    def nkptPBZ(self):
-        '''
-        Return number of PC kpoints.
-        '''
-        return(self.PBZ_kpts_list_org.shape[0])
-
-    @property
-    def nkptPBZ_unique(self):
-        '''
-        Return number of PC kpoints.
-        '''
-        return(self.PBZ_kpts_list.shape[0])
-    
-    def _print_info(self, level='low'):
-        """
-        Printing information about the band folding.
-        
-        Percentage folding = ((#of PC kpoints - #of folded SC Kpoints)/(#of PC kpoints))*100
-
-        Parameters
-        ----------
-        level : ['low','medium','high'], optional
-            Level of printing information. The default is 'low'.
-
-        Returns
-        -------
-        None.
-
-        """
-        print(f"{'='*_draw_line_length}\n- Folding info:")
-        print(f"-- Total number of unique PC kpoints: {self.nkptPBZ} ({self.nkptPBZ_unique} unique)")
-        print(f"-- {self.nkptPBZ_unique} unique PC k-points => {self.nkptSBZ} unique SC K-points")
-        print(f'-- Percentage folding: {(self.nkptPBZ_unique-self.nkptSBZ)/self.nkptPBZ_unique*100:.3f} %')
-        if level in ['medium','high']:
-            print(f"{'='*_draw_line_length}")
-            print(f'- Special k-points (pos_index, label): {self.special_kpoints_pos_labels}')
-            if level == 'high':
-                self._print_PBZ_SBZ_kpts_mapping_full()
-            else:
-                self._print_PBZ_SBZ_kpts_mapping()
-
-    def kpoints_SBZ_str(self):
-        """
-        Create string of SC kpoints generated.
-
-        Returns
-        -------
-        str
-            String of SC kpoints generated..
-
-        """
-        return f"{self.nkptSBZ}\n"+"\n".join("  ".join(f"{x:12.8f}" for x in k ) 
-                                                     for k in self.SBZ_kpts_list)+"\n"
-    
-    def _get_PBZ_SBZ_kpts_mapping(self):
-        """
-        Find mapping of SC kpoints to PC kpoints.
-
-        Returns
-        -------
-        None.
-
-        """
-        self.SBZ_PBZ_kpts_mapping = {}
-        
-        for i in np.unique(self.kpointsSBZ_index_in_unique):
-            self.SBZ_PBZ_kpts_mapping[i] = {}
-            for mm in np.argwhere(self.kpointsSBZ_index_in_unique==i).flatten():
-                self.SBZ_PBZ_kpts_mapping[i][mm] = []
-                for kk in np.argwhere(self.kpointsPBZ_index_in_unique==mm).flatten():
-                    self.SBZ_PBZ_kpts_mapping[i][mm].append(kk)
-        return 
-    
-    def _print_PBZ_SBZ_kpts_mapping(self):
-        """
-        Print mapping of SC kpoints to PC kpoints.
-
-        Returns
-        -------
-        None.
-
-        """
-        print(f"{'='*_draw_line_length}\n- K-k relation: (K index: K -> k index: k)")
-        for key, val in self.SBZ_PBZ_kpts_mapping.items(): # key: SC-kp index; val: list of unique PC-kpts indices
-            print(f"-- {key:>5}:" + "  ".join(f"{x:12.8f}" for x in self.SBZ_kpts_list[key][:3]))
-            for _, vall in val.items(): # kkk: unique PC-kpts indices; vall: list of PC-kpts indices
-                    for kk in vall:
-                            print(f"\t--- {kk:>5}:" + "  ".join(f"{x:12.8f}" for x in self.PBZ_kpts_list_org[kk, :3]))
-    
-    def _print_PBZ_SBZ_kpts_mapping_full(self):
-        """
-        Print mapping of SC kpoints to PC kpoints.
-
-        Returns
-        -------
-        None.
-
-        """
-        print(f"{'='*_draw_line_length}\n- K-k relation: (K index: K -> k index unique: k unique -> k index: k)")
-        for key, val in self.SBZ_PBZ_kpts_mapping.items(): # key: SC-kp index; val: list of unique PC-kpts indices
-            print(f"-- {key:>5}:" + "  ".join(f"{x:12.8f}" for x in self.SBZ_kpts_list[key, :3]))
-            for kkk, vall in val.items(): # kkk: unique PC-kpts indices; vall: list of PC-kpts indices
-                    print(f"\t--- {kkk:>5}:" + "  ".join(f"{x:12.8f}" for x in self.PBZ_kpts_list[kkk, :3]))
-                    for kk in vall:
-                            print(f"\t\t---- {kk:>5}:" + "  ".join(f"{x:12.8f}" for x in self.PBZ_kpts_list_org[kk, :3]))
+import numpy as np
+from ..BasicFunctions.general_functions import _draw_line_length
+    
+### ===========================================================================
+class FindProperties:
+    def __init__(self):
+        pass
+    
+    @property
+    def nkptSBZ(self):
+        '''
+        Return number of (unique) SC kpoints.
+        '''
+        return(self.SBZ_kpts_list.shape[0])
+    
+    @property
+    def nkptPBZ(self):
+        '''
+        Return number of PC kpoints.
+        '''
+        return(self.PBZ_kpts_list_org.shape[0])
+
+    @property
+    def nkptPBZ_unique(self):
+        '''
+        Return number of PC kpoints.
+        '''
+        return(self.PBZ_kpts_list.shape[0])
+    
+    def _print_info(self, level='low'):
+        """
+        Printing information about the band folding.
+        
+        Percentage folding = ((#of PC kpoints - #of folded SC Kpoints)/(#of PC kpoints))*100
+
+        Parameters
+        ----------
+        level : ['low','medium','high'], optional
+            Level of printing information. The default is 'low'.
+
+        Returns
+        -------
+        None.
+
+        """
+        print(f"{'='*_draw_line_length}\n- Folding info:")
+        print(f"-- Total number of unique PC kpoints: {self.nkptPBZ} ({self.nkptPBZ_unique} unique)")
+        print(f"-- {self.nkptPBZ_unique} unique PC k-points => {self.nkptSBZ} unique SC K-points")
+        print(f'-- Percentage folding: {(self.nkptPBZ_unique-self.nkptSBZ)/self.nkptPBZ_unique*100:.3f} %')
+        if level in ['medium','high']:
+            print(f"{'='*_draw_line_length}")
+            print(f'- Special k-points (pos_index, label): {self.special_kpoints_pos_labels}')
+            if level == 'high':
+                self._print_PBZ_SBZ_kpts_mapping_full()
+            else:
+                self._print_PBZ_SBZ_kpts_mapping()
+
+    def kpoints_SBZ_str(self):
+        """
+        Create string of SC kpoints generated.
+
+        Returns
+        -------
+        str
+            String of SC kpoints generated..
+
+        """
+        return f"{self.nkptSBZ}\n"+"\n".join("  ".join(f"{x:12.8f}" for x in k ) 
+                                                     for k in self.SBZ_kpts_list)+"\n"
+    
+    def _get_PBZ_SBZ_kpts_mapping(self):
+        """
+        Find mapping of SC kpoints to PC kpoints.
+
+        Returns
+        -------
+        None.
+
+        """
+        self.SBZ_PBZ_kpts_mapping = {}
+        
+        for i in np.unique(self.kpointsSBZ_index_in_unique):
+            self.SBZ_PBZ_kpts_mapping[i] = {}
+            for mm in np.argwhere(self.kpointsSBZ_index_in_unique==i).flatten():
+                self.SBZ_PBZ_kpts_mapping[i][mm] = []
+                for kk in np.argwhere(self.kpointsPBZ_index_in_unique==mm).flatten():
+                    self.SBZ_PBZ_kpts_mapping[i][mm].append(kk)
+        return 
+    
+    def _print_PBZ_SBZ_kpts_mapping(self):
+        """
+        Print mapping of SC kpoints to PC kpoints.
+
+        Returns
+        -------
+        None.
+
+        """
+        print(f"{'='*_draw_line_length}\n- K-k relation: (K index: K -> k index: k)")
+        for key, val in self.SBZ_PBZ_kpts_mapping.items(): # key: SC-kp index; val: list of unique PC-kpts indices
+            print(f"-- {key:>5}:" + "  ".join(f"{x:12.8f}" for x in self.SBZ_kpts_list[key][:3]))
+            for _, vall in val.items(): # kkk: unique PC-kpts indices; vall: list of PC-kpts indices
+                    for kk in vall:
+                            print(f"\t--- {kk:>5}:" + "  ".join(f"{x:12.8f}" for x in self.PBZ_kpts_list_org[kk, :3]))
+    
+    def _print_PBZ_SBZ_kpts_mapping_full(self):
+        """
+        Print mapping of SC kpoints to PC kpoints.
+
+        Returns
+        -------
+        None.
+
+        """
+        print(f"{'='*_draw_line_length}\n- K-k relation: (K index: K -> k index unique: k unique -> k index: k)")
+        for key, val in self.SBZ_PBZ_kpts_mapping.items(): # key: SC-kp index; val: list of unique PC-kpts indices
+            print(f"-- {key:>5}:" + "  ".join(f"{x:12.8f}" for x in self.SBZ_kpts_list[key, :3]))
+            for kkk, vall in val.items(): # kkk: unique PC-kpts indices; vall: list of PC-kpts indices
+                    print(f"\t--- {kkk:>5}:" + "  ".join(f"{x:12.8f}" for x in self.PBZ_kpts_list[kkk, :3]))
+                    for kk in vall:
+                            print(f"\t\t---- {kk:>5}:" + "  ".join(f"{x:12.8f}" for x in self.PBZ_kpts_list_org[kk, :3]))
```

### Comparing `banduppy-0.3.0/banduppy/src/unfolding.py` & `banduppy-0.3.1/banduppy/src/unfolding.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,359 +1,358 @@
-import numpy as np
-from ..BasicFunctions.general_functions import SaveData2File, _BasicFunctionsModule, _draw_line_length
-from .._version import _pkg_version
-try:
-    from irrep.__aux import is_round
-except ImportError:
-    from irrep.utility import is_round
-
-### ===========================================================================
-class BandUnfolding:
-    """
-    Band unfolding from supercell to primitive cell band structure (effective band structure).
-
-    """
-    
-    def __init__(self, supercell, PBZ_kpts_list_full,  
-                 SBZ_kpts_list, SBZ_PBZ_kpts_map, 
-                 print_info='low'):
-        """
-        Initializing the unfolding class.
-
-        Parameters
-        ----------
-        supercell : 3X3 matrix
-            Primitive-to-supercell transformation matrix.
-        PBZ_kpts_list_full : ndarray of floats
-            PC kpoints list (orginal provided k-path, full list).
-        SBZ_kpts_list : ndarray of float
-            SC kpoints list (unique).
-        SBZ_PBZ_kpts_map : dictionary of int/list
-            Mapping of SC kpts (K), PC unique kpts (k unique), and PC full kpts (k) indices.
-            format: {K index: K -> k index unique: k unique -> k index: k}
-            This mapping is used for reverse engineer latter.
-        print_info : [None,'low','medium','high'], optional
-            Print information of kpoints folding. Level of printing information. 
-            The default is 'low'. If None, nothing is printed.
-
-        """
-        self.transformation_matrix = _BasicFunctionsModule._check_transformation_matrix(np.array(supercell))
-        self.kpointsPBZ_full = _BasicFunctionsModule._round_2_tolerance(PBZ_kpts_list_full) 
-        self.kpointsSBZ = _BasicFunctionsModule._round_2_tolerance(SBZ_kpts_list)
-        self.SBZ_PBZ_kpts_index_map = SBZ_PBZ_kpts_map
-        self.print_information = print_info
-
-    
-    def _gather_generated_ab_calculated_kpts(self, wavefns_file_kpts):
-        """
-        Collect Kpoints in the generated SC-Kpoints list those only exist in the 
-        wavefunction file from ab-initio calculation. 
-        
-        Note: This way you can do sections of k-paths in ab-initio calculations to avoid
-        large calculations. Carefully check the WARNING msgs.
-        
-        Note: Quick theory:
-        If SC reciprocal lattice =  G(k<-K) 
-        o K unfold onto k with the unfolding vector G(k<-K). One K can unfold to multiple k.
-        o But a given k can fold to only one K.
-
-        Parameters
-        ----------
-        wavefns_file_kpts : irrep.kpoint.Kpoint
-            List of irrep.kpoint.Kpoint from ab-initio calculations.
-
-        Calculates
-        -------
-        kpSBZcalc Dictionary = 
-            {SC-Kpoint index: 
-                 unfolded PC-kpoint index: (band energy, Bloch weights).}
-
-        """
-        self.kpSBZcalc = {}
-        for key, val in self.SBZ_PBZ_kpts_index_map.items(): # Loop over all SC-Kpoints
-            found = False
-            for KP in wavefns_file_kpts:
-                # Check if K exists in wavefunction file K-list
-                if is_round(KP.K - self.kpointsSBZ[key, :3], prec = 1e-6):
-                    self.kpSBZcalc[key] = {}
-                    for vall in val.values(): # Loop over PC-kpoints
-                        for kk in vall:
-                            # Calculate weights for the PBZ kpoints from SBZ kpoints on which
-                            # it was folded.
-                            # If SC reciprocal lattice =  G(k<-K) 
-                            # o K unfold onto k with the unfolding vector G(k<-K). One K can unfold to multiple k.
-                            # o But a given k can fold to only one K.
-                            self.kpSBZcalc[key][kk] = KP.unfold(supercell=self.transformation_matrix, 
-                                                                kptPBZ=self.kpointsPBZ_full[kk, :3])
-                    found = True
-            if not found:
-                print("WARNING: SC K-point "+f"{key:>5}"+"  ".join(f"{kpp:12.8f}" for kpp in self.kpointsSBZ[key])+" was not found in the calculated bandstructure.")
-                print("- The corresponding following PC-kpoints in the unfolding path will be skipped:")
-                for _, vall in val.items(): # kkk: unique PC-kpts indices; vall: list of PC-kpts indices
-                    for kk in vall:
-                            print(f"\t--- {kk:>5}:" + "  ".join(f"{x:12.8f}" for x in self.kpointsPBZ_full[kk, :3])) 
-    
-    def _unfold_bandstructure(self, bandstructure, break_thresh = 0.1):  
-        """
-        
-
-        Parameters
-        ----------
-        bandstructure : irrep.bandstructure.BandStructure
-            irrep.bandstructure.BandStructure data.
-        break_thresh : float, optional
-            If the distance between two neighboring k-points in the path is 
-            larger than `break_thresh` break continuity in k-path. Set break_thresh 
-            to a large value if the unfolded kpoints line is continuous.
-            The default is 0.1.
-
-        Returns
-        -------
-        None.
-
-        """            
-        # Check/return if kpoints in the generated SC-kpoints list exists in the
-        # wavefunction file from ab-initio calculation.
-        _ = self._gather_generated_ab_calculated_kpts(bandstructure.kpoints)
-        
-        # Collect all unfolded PBZ kpoints, energy and weights from calculated kpSBZcalc dictionary
-        kpPBZ_unfolded = {k: v for val in self.kpSBZcalc.values() for k, v in val.items()} 
-        # Sort the unfolded PBZ
-        kpPBZ_unfolded = {k: v for k, v in sorted(kpPBZ_unfolded.items(), key=lambda item: item[0])}
-
-        # This makes sure when you do section by section DFT band structures
-        # then read only read part of it.
-        # k-index, k1, k2, k3
-        self.unfolded_kpts_dat = np.array([[kk]+list(self.kpointsPBZ_full[kk, :3]) 
-                                           for kk in kpPBZ_unfolded])
-        #self.unfolded_kpts_dat = unfolded_kpts_dat_[unfolded_kpts_dat_[:, 0].argsort()] # No need any more
-        self.kpline = bandstructure.KPOINTSline(kpred=self.unfolded_kpts_dat[:,1:], breakTHRESH=break_thresh)
-        # # Converting k-indices to k on path (A^-1)
-        # self.unfolded_kpts_dat[:,0] = self.kpline
-        
-        # Insert k on path (A^-1) after k-indices
-        self.unfolded_kpts_dat = np.insert(self.unfolded_kpts_dat,1, self.kpline, axis=1)
-        
-        # # Add k-path to the energy, weight band structure array
-        # self.unfolded_bandstructure = np.concatenate([np.insert(unf, 0, self.kpline[kk], axis=1) 
-        #                                               for kk, unf in kpPBZ_unfolded.items()], axis=0)
-        
-        # Add k-indices and k-path to the energy, weight band structure array
-        self.unfolded_bandstructure = np.concatenate([np.insert(unf, [0, 0], [kk, self.kpline[kk]], axis=1) 
-                                                      for kk, unf in kpPBZ_unfolded.items()], axis=0)
-        
-        # Print information about folding
-        if self.print_information is not None: 
-            self._print_info_post(level=self.print_information)          
-        return
-    
-    def _print_Post_unfolded_PBZ_kpts(self):
-        """
-        Print the unfolded k-points.
-
-        Returns
-        -------
-        None.
-
-        """
-        print(f"{'='*_draw_line_length}\n- Unfolded PC k-points from postprocessed wavefunction file:[k on path (A^-1), k1, k2, k3]")
-        for val in self.unfolded_kpts_dat:
-                print('-- '+"  ".join(f"{x:12.8f}" for x in val[1:]))
-
-    def _print_info_post(self, level='low'):
-        """
-        Printing information about the unfolding (e.g. unfolded k-points).
-
-        Parameters
-        ----------
-        level : ['low','medium','high'], optional
-            Level of printing information. The default is 'low'.
-
-        Returns
-        -------
-        None.
-
-        """
-        if level == 'high':
-            self._print_Post_unfolded_PBZ_kpts()
-                    
-    def _save_Post_unfolded_PBZ_kpts(self, save_dir, file_name, file_name_suffix):
-        """
-        Save unfolded PC-kpoints.
-        Format: k-index, k on path (A^-1), k1, k2, k3
-
-        Parameters
-        ----------
-        save_dir : str or path
-            Directory path where to save the file.
-        file_name : str
-            Name of the file.
-        file_name_suffix : str
-            Suffix to add to the file name.
-
-        Returns
-        -------
-        None.
-
-        """
-        if self.print_information is not None: 
-            print(f"{'='*_draw_line_length}\n- Saving unfolded kpoints to file...")
-        header_msg  = " Unfolded PC k-points from postprocessed wavefunction file\n"
-        header_msg += " k-index, k on path (A^-1), k1, k2, k3\n"
-        # Save the sc-kpoints in file
-        save_f_name = \
-        SaveData2File.save_2_file(data=self.unfolded_kpts_dat, 
-                                  save_dir=save_dir, file_name=file_name,
-                                  file_name_suffix=f'{file_name_suffix}.dat', 
-                                  header_txt=header_msg, comments_symbol='#',
-                                  print_log=bool(self.print_information))
-        if self.print_information is not None: 
-            print(f'-- Filepath: {save_f_name}\n- Done')
-        
-    def _save_Post_unfolded_bandstucture(self, save_dir, file_name, file_name_suffix, is_spinor:bool=False):
-        """
-        Save unfolded effective band structure data.
-        Format: k-index, k on path (A^-1), k1, k2, k3
-
-        Parameters
-        ----------
-        save_dir : str or path
-            Directory path where to save the file.
-        file_name : str
-            Name of the file.
-        file_name_suffix : str
-            Suffix to add to the file name.
-        is_spinor : bool, optional
-            If the bands in wave function files are non-degenerate (spinor). 
-            The default is False.
-
-        Returns
-        -------
-        None.
-
-        """
-        if self.print_information is not None: 
-            print(f"{'='*_draw_line_length}\n- Saving unfolded bandstructure to file...")
-        header_msg  = " Unfolded band structure from postprocessed wavefunction file\n"
-        header_msg += " k-index, k on path (A^-1), energy, weight " + \
-                        ("Sx,Sy,Sz" if is_spinor else "")  +"\n"
-        # Save the unfolded band structure in file
-        save_f_name = \
-        SaveData2File.save_2_file(data=self.unfolded_bandstructure, 
-                                  save_dir=save_dir, file_name=file_name,
-                                  file_name_suffix=f'{file_name_suffix}.dat', 
-                                  header_txt=header_msg, comments_symbol='#',
-                                  print_log=bool(self.print_information)) #,
-                                  #np_data_fmt='%.18e')
-        if self.print_information is not None: 
-            print(f'-- Filepath: {save_f_name}\n- Done')
-            
-    def _save_unfolded_kpts_bandstr(self,
-                                    save_unfolded_kpts = {'save2file': False,
-                                                          'fdir': '.',
-                                                          'fname': 'kpoints_unfolded',
-                                                          'fname_suffix': ''},
-                                    save_unfolded_bandstr = {'save2file': False, 
-                                                             'fdir': '.',
-                                                             'fname': 'bandstructure_unfolded',
-                                                             'fname_suffix': ''}): 
-        """
-        Save the unfolded kpoints and band structure data.
-
-        Parameters
-        ----------
-        save_unfolded_kpts : dictionary, optional
-            save2file :: Save unfolded kpoints or not? 
-            fir :: str or path
-                Directory path where to save the file.
-            fname :: str
-                Name of the file.
-            fname_suffix :: str
-                Suffix to add to the file name.
-            The default is {'save2file': False, 'fdir': '.', 'fname': 'kpoints_unfolded', 'fname_suffix': ''}.
-        save_unfolded_bandstr : dictionary, optional
-            save2file :: Save unfolded kpoints or not? 
-            fir :: str or path
-                Directory path where to save the file.
-            fname :: str
-                Name of the file.
-            fname_suffix :: str
-                Suffix to add to the file name. 
-            The default is {'save2file': False, 'fdir': '.', 'fname': 'bandstructure_unfolded', 'fname_suffix': ''}.
-
-        Returns
-        -------
-        None.
-
-        """
-        # Save unfolded kpoints after post processing of wave function file
-        if save_unfolded_kpts['save2file']:
-            self._save_Post_unfolded_PBZ_kpts(save_dir=save_unfolded_kpts["fdir"], 
-                                              file_name=save_unfolded_kpts["fname"], 
-                                              file_name_suffix=save_unfolded_kpts["fname_suffix"])
-        # Save unfolded band structure after post processing of wave function file
-        if save_unfolded_bandstr['save2file']:
-            self._save_Post_unfolded_bandstucture(save_dir=save_unfolded_bandstr["fdir"], 
-                                                  file_name=save_unfolded_bandstr["fname"], 
-                                                  file_name_suffix=save_unfolded_bandstr["fname_suffix"])
-
-    def unfold(self, bandstructure, kline_discontinuity_threshold = 0.1,
-               save_unfolded_kpts = {'save2file': False, 
-                                     'fdir': '.',
-                                     'fname': 'kpoints_unfolded',
-                                     'fname_suffix': ''},
-               save_unfolded_bandstr = {'save2file': False, 
-                                        'fdir': '.',
-                                        'fname': 'bandstructure_unfolded',
-                                        'fname_suffix': ''}): 
-        """
-        
-
-        Parameters
-        ----------
-        bandstructure : irrep.bandstructure.BandStructure
-            irrep.bandstructure.BandStructure.
-        kline_discontinuity_threshold : float, optional
-            If the distance between two neighboring k-points in the path is 
-            larger than `break_thresh` break continuity in k-path. Set break_thresh 
-            to a large value if the unfolded kpoints line is continuous.
-            The default is 0.1.
-        save_unfolded_kpts : dictionary, optional
-            save2file :: Save unfolded kpoints or not? 
-            fir :: str or path
-                Directory path where to save the file.
-            fname :: str
-                Name of the file.
-            fname_suffix :: str
-                Suffix to add to the file name.
-            The default is {'save2file': False, 'fdir': '.', 'fname': 'kpoints_unfolded', 'fname_suffix': ''}.
-        save_unfolded_bandstr : dictionary, optional
-            save2file :: Save unfolded kpoints or not? 
-            fir :: str or path
-                Directory path where to save the file.
-            fname :: str
-                Name of the file.
-            fname_suffix :: str
-                Suffix to add to the file name. 
-            The default is {'save2file': False, 'fdir': '.', 'fname': 'bandstructure_unfolded', 'fname_suffix': ''}.
-            
-        Returns
-        -------
-        numpy ndarray
-            Unfolded effective band structure.
-            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
-        numpy ndarray
-            Unfolded effective band structure k-path.
-            Format: k on path (A^-1)
-
-        """
-        # kline_discontinuity_threshold: float, default=0.1
-        #    If the distance between two neighboring k-points in the path is 
-        #    larger than `kline_discontinuity_threshold`, it is taken to be 0.
-        # Set kline_discontinuity_threshold to a large value if the unfolded kpoints line is continuous
-        # Unfold bandstructure
-        self._unfold_bandstructure(bandstructure, break_thresh=kline_discontinuity_threshold)
-        
-        # Save unfolded kpoints after post processing of wave function file
-        self._save_unfolded_kpts_bandstr(save_unfolded_kpts, save_unfolded_bandstr)
-        
-        return self.unfolded_bandstructure, self.kpline
+import numpy as np
+from ..BasicFunctions.general_functions import SaveData2File, _BasicFunctionsModule, _draw_line_length
+try:
+    from irrep.__aux import is_round
+except ImportError:
+    from irrep.utility import is_round
+
+### ===========================================================================
+class BandUnfolding:
+    """
+    Band unfolding from supercell to primitive cell band structure (effective band structure).
+
+    """
+    
+    def __init__(self, supercell, PBZ_kpts_list_full,  
+                 SBZ_kpts_list, SBZ_PBZ_kpts_map, 
+                 print_info='low'):
+        """
+        Initializing the unfolding class.
+
+        Parameters
+        ----------
+        supercell : 3X3 matrix
+            Primitive-to-supercell transformation matrix.
+        PBZ_kpts_list_full : ndarray of floats
+            PC kpoints list (orginal provided k-path, full list).
+        SBZ_kpts_list : ndarray of float
+            SC kpoints list (unique).
+        SBZ_PBZ_kpts_map : dictionary of int/list
+            Mapping of SC kpts (K), PC unique kpts (k unique), and PC full kpts (k) indices.
+            format: {K index: K -> k index unique: k unique -> k index: k}
+            This mapping is used for reverse engineer latter.
+        print_info : [None,'low','medium','high'], optional
+            Print information of kpoints folding. Level of printing information. 
+            The default is 'low'. If None, nothing is printed.
+
+        """
+        self.transformation_matrix = _BasicFunctionsModule._check_transformation_matrix(np.array(supercell))
+        self.kpointsPBZ_full = _BasicFunctionsModule._round_2_tolerance(PBZ_kpts_list_full) 
+        self.kpointsSBZ = _BasicFunctionsModule._round_2_tolerance(SBZ_kpts_list)
+        self.SBZ_PBZ_kpts_index_map = SBZ_PBZ_kpts_map
+        self.print_information = print_info
+
+    
+    def _gather_generated_ab_calculated_kpts(self, wavefns_file_kpts):
+        """
+        Collect Kpoints in the generated SC-Kpoints list those only exist in the 
+        wavefunction file from ab-initio calculation. 
+        
+        Note: This way you can do sections of k-paths in ab-initio calculations to avoid
+        large calculations. Carefully check the WARNING msgs.
+        
+        Note: Quick theory:
+        If SC reciprocal lattice =  G(k<-K) 
+        o K unfold onto k with the unfolding vector G(k<-K). One K can unfold to multiple k.
+        o But a given k can fold to only one K.
+
+        Parameters
+        ----------
+        wavefns_file_kpts : irrep.kpoint.Kpoint
+            List of irrep.kpoint.Kpoint from ab-initio calculations.
+
+        Calculates
+        -------
+        kpSBZcalc Dictionary = 
+            {SC-Kpoint index: 
+                 unfolded PC-kpoint index: (band energy, Bloch weights).}
+
+        """
+        self.kpSBZcalc = {}
+        for key, val in self.SBZ_PBZ_kpts_index_map.items(): # Loop over all SC-Kpoints
+            found = False
+            for KP in wavefns_file_kpts:
+                # Check if K exists in wavefunction file K-list
+                if is_round(KP.K - self.kpointsSBZ[key, :3], prec = 1e-6):
+                    self.kpSBZcalc[key] = {}
+                    for vall in val.values(): # Loop over PC-kpoints
+                        for kk in vall:
+                            # Calculate weights for the PBZ kpoints from SBZ kpoints on which
+                            # it was folded.
+                            # If SC reciprocal lattice =  G(k<-K) 
+                            # o K unfold onto k with the unfolding vector G(k<-K). One K can unfold to multiple k.
+                            # o But a given k can fold to only one K.
+                            self.kpSBZcalc[key][kk] = KP.unfold(supercell=self.transformation_matrix, 
+                                                                kptPBZ=self.kpointsPBZ_full[kk, :3])
+                    found = True
+            if not found:
+                print("WARNING: SC K-point "+f"{key:>5}"+"  ".join(f"{kpp:12.8f}" for kpp in self.kpointsSBZ[key])+" was not found in the calculated bandstructure.")
+                print("- The corresponding following PC-kpoints in the unfolding path will be skipped:")
+                for _, vall in val.items(): # kkk: unique PC-kpts indices; vall: list of PC-kpts indices
+                    for kk in vall:
+                            print(f"\t--- {kk:>5}:" + "  ".join(f"{x:12.8f}" for x in self.kpointsPBZ_full[kk, :3])) 
+    
+    def _unfold_bandstructure(self, bandstructure, break_thresh = 0.1):  
+        """
+        
+
+        Parameters
+        ----------
+        bandstructure : irrep.bandstructure.BandStructure
+            irrep.bandstructure.BandStructure data.
+        break_thresh : float, optional
+            If the distance between two neighboring k-points in the path is 
+            larger than `break_thresh` break continuity in k-path. Set break_thresh 
+            to a large value if the unfolded kpoints line is continuous.
+            The default is 0.1.
+
+        Returns
+        -------
+        None.
+
+        """            
+        # Check/return if kpoints in the generated SC-kpoints list exists in the
+        # wavefunction file from ab-initio calculation.
+        _ = self._gather_generated_ab_calculated_kpts(bandstructure.kpoints)
+        
+        # Collect all unfolded PBZ kpoints, energy and weights from calculated kpSBZcalc dictionary
+        kpPBZ_unfolded = {k: v for val in self.kpSBZcalc.values() for k, v in val.items()} 
+        # Sort the unfolded PBZ
+        kpPBZ_unfolded = {k: v for k, v in sorted(kpPBZ_unfolded.items(), key=lambda item: item[0])}
+
+        # This makes sure when you do section by section DFT band structures
+        # then read only read part of it.
+        # k-index, k1, k2, k3
+        self.unfolded_kpts_dat = np.array([[kk]+list(self.kpointsPBZ_full[kk, :3]) 
+                                           for kk in kpPBZ_unfolded])
+        #self.unfolded_kpts_dat = unfolded_kpts_dat_[unfolded_kpts_dat_[:, 0].argsort()] # No need any more
+        self.kpline = bandstructure.KPOINTSline(kpred=self.unfolded_kpts_dat[:,1:], breakTHRESH=break_thresh)
+        # # Converting k-indices to k on path (A^-1)
+        # self.unfolded_kpts_dat[:,0] = self.kpline
+        
+        # Insert k on path (A^-1) after k-indices
+        self.unfolded_kpts_dat = np.insert(self.unfolded_kpts_dat,1, self.kpline, axis=1)
+        
+        # # Add k-path to the energy, weight band structure array
+        # self.unfolded_bandstructure = np.concatenate([np.insert(unf, 0, self.kpline[kk], axis=1) 
+        #                                               for kk, unf in kpPBZ_unfolded.items()], axis=0)
+        
+        # Add k-indices and k-path to the energy, weight band structure array
+        self.unfolded_bandstructure = np.concatenate([np.insert(unf, [0, 0], [kk, self.kpline[kk]], axis=1) 
+                                                      for kk, unf in kpPBZ_unfolded.items()], axis=0)
+        
+        # Print information about folding
+        if self.print_information is not None: 
+            self._print_info_post(level=self.print_information)          
+        return
+    
+    def _print_Post_unfolded_PBZ_kpts(self):
+        """
+        Print the unfolded k-points.
+
+        Returns
+        -------
+        None.
+
+        """
+        print(f"{'='*_draw_line_length}\n- Unfolded PC k-points from postprocessed wavefunction file:[k on path (A^-1), k1, k2, k3]")
+        for val in self.unfolded_kpts_dat:
+                print('-- '+"  ".join(f"{x:12.8f}" for x in val[1:]))
+
+    def _print_info_post(self, level='low'):
+        """
+        Printing information about the unfolding (e.g. unfolded k-points).
+
+        Parameters
+        ----------
+        level : ['low','medium','high'], optional
+            Level of printing information. The default is 'low'.
+
+        Returns
+        -------
+        None.
+
+        """
+        if level == 'high':
+            self._print_Post_unfolded_PBZ_kpts()
+                    
+    def _save_Post_unfolded_PBZ_kpts(self, save_dir, file_name, file_name_suffix):
+        """
+        Save unfolded PC-kpoints.
+        Format: k-index, k on path (A^-1), k1, k2, k3
+
+        Parameters
+        ----------
+        save_dir : str or path
+            Directory path where to save the file.
+        file_name : str
+            Name of the file.
+        file_name_suffix : str
+            Suffix to add to the file name.
+
+        Returns
+        -------
+        None.
+
+        """
+        if self.print_information is not None: 
+            print(f"{'='*_draw_line_length}\n- Saving unfolded kpoints to file...")
+        header_msg  = " Unfolded PC k-points from postprocessed wavefunction file\n"
+        header_msg += " k-index, k on path (A^-1), k1, k2, k3\n"
+        # Save the sc-kpoints in file
+        save_f_name = \
+        SaveData2File.save_2_file(data=self.unfolded_kpts_dat, 
+                                  save_dir=save_dir, file_name=file_name,
+                                  file_name_suffix=f'{file_name_suffix}.dat', 
+                                  header_txt=header_msg, comments_symbol='#',
+                                  print_log=bool(self.print_information))
+        if self.print_information is not None: 
+            print(f'-- Filepath: {save_f_name}\n- Done')
+        
+    def _save_Post_unfolded_bandstucture(self, save_dir, file_name, file_name_suffix, is_spinor:bool=False):
+        """
+        Save unfolded effective band structure data.
+        Format: k-index, k on path (A^-1), k1, k2, k3
+
+        Parameters
+        ----------
+        save_dir : str or path
+            Directory path where to save the file.
+        file_name : str
+            Name of the file.
+        file_name_suffix : str
+            Suffix to add to the file name.
+        is_spinor : bool, optional
+            If the bands in wave function files are non-degenerate (spinor). 
+            The default is False.
+
+        Returns
+        -------
+        None.
+
+        """
+        if self.print_information is not None: 
+            print(f"{'='*_draw_line_length}\n- Saving unfolded bandstructure to file...")
+        header_msg  = " Unfolded band structure from postprocessed wavefunction file\n"
+        header_msg += " k-index, k on path (A^-1), energy, weight " + \
+                        ("Sx,Sy,Sz" if is_spinor else "")  +"\n"
+        # Save the unfolded band structure in file
+        save_f_name = \
+        SaveData2File.save_2_file(data=self.unfolded_bandstructure, 
+                                  save_dir=save_dir, file_name=file_name,
+                                  file_name_suffix=f'{file_name_suffix}.dat', 
+                                  header_txt=header_msg, comments_symbol='#',
+                                  print_log=bool(self.print_information)) #,
+                                  #np_data_fmt='%.18e')
+        if self.print_information is not None: 
+            print(f'-- Filepath: {save_f_name}\n- Done')
+            
+    def _save_unfolded_kpts_bandstr(self,
+                                    save_unfolded_kpts = {'save2file': False,
+                                                          'fdir': '.',
+                                                          'fname': 'kpoints_unfolded',
+                                                          'fname_suffix': ''},
+                                    save_unfolded_bandstr = {'save2file': False, 
+                                                             'fdir': '.',
+                                                             'fname': 'bandstructure_unfolded',
+                                                             'fname_suffix': ''}): 
+        """
+        Save the unfolded kpoints and band structure data.
+
+        Parameters
+        ----------
+        save_unfolded_kpts : dictionary, optional
+            save2file :: Save unfolded kpoints or not? 
+            fir :: str or path
+                Directory path where to save the file.
+            fname :: str
+                Name of the file.
+            fname_suffix :: str
+                Suffix to add to the file name.
+            The default is {'save2file': False, 'fdir': '.', 'fname': 'kpoints_unfolded', 'fname_suffix': ''}.
+        save_unfolded_bandstr : dictionary, optional
+            save2file :: Save unfolded kpoints or not? 
+            fir :: str or path
+                Directory path where to save the file.
+            fname :: str
+                Name of the file.
+            fname_suffix :: str
+                Suffix to add to the file name. 
+            The default is {'save2file': False, 'fdir': '.', 'fname': 'bandstructure_unfolded', 'fname_suffix': ''}.
+
+        Returns
+        -------
+        None.
+
+        """
+        # Save unfolded kpoints after post processing of wave function file
+        if save_unfolded_kpts['save2file']:
+            self._save_Post_unfolded_PBZ_kpts(save_dir=save_unfolded_kpts["fdir"], 
+                                              file_name=save_unfolded_kpts["fname"], 
+                                              file_name_suffix=save_unfolded_kpts["fname_suffix"])
+        # Save unfolded band structure after post processing of wave function file
+        if save_unfolded_bandstr['save2file']:
+            self._save_Post_unfolded_bandstucture(save_dir=save_unfolded_bandstr["fdir"], 
+                                                  file_name=save_unfolded_bandstr["fname"], 
+                                                  file_name_suffix=save_unfolded_bandstr["fname_suffix"])
+
+    def unfold(self, bandstructure, kline_discontinuity_threshold = 0.1,
+               save_unfolded_kpts = {'save2file': False, 
+                                     'fdir': '.',
+                                     'fname': 'kpoints_unfolded',
+                                     'fname_suffix': ''},
+               save_unfolded_bandstr = {'save2file': False, 
+                                        'fdir': '.',
+                                        'fname': 'bandstructure_unfolded',
+                                        'fname_suffix': ''}): 
+        """
+        
+
+        Parameters
+        ----------
+        bandstructure : irrep.bandstructure.BandStructure
+            irrep.bandstructure.BandStructure.
+        kline_discontinuity_threshold : float, optional
+            If the distance between two neighboring k-points in the path is 
+            larger than `break_thresh` break continuity in k-path. Set break_thresh 
+            to a large value if the unfolded kpoints line is continuous.
+            The default is 0.1.
+        save_unfolded_kpts : dictionary, optional
+            save2file :: Save unfolded kpoints or not? 
+            fir :: str or path
+                Directory path where to save the file.
+            fname :: str
+                Name of the file.
+            fname_suffix :: str
+                Suffix to add to the file name.
+            The default is {'save2file': False, 'fdir': '.', 'fname': 'kpoints_unfolded', 'fname_suffix': ''}.
+        save_unfolded_bandstr : dictionary, optional
+            save2file :: Save unfolded kpoints or not? 
+            fir :: str or path
+                Directory path where to save the file.
+            fname :: str
+                Name of the file.
+            fname_suffix :: str
+                Suffix to add to the file name. 
+            The default is {'save2file': False, 'fdir': '.', 'fname': 'bandstructure_unfolded', 'fname_suffix': ''}.
+            
+        Returns
+        -------
+        numpy ndarray
+            Unfolded effective band structure.
+            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
+        numpy ndarray
+            Unfolded effective band structure k-path.
+            Format: k on path (A^-1)
+
+        """
+        # kline_discontinuity_threshold: float, default=0.1
+        #    If the distance between two neighboring k-points in the path is 
+        #    larger than `kline_discontinuity_threshold`, it is taken to be 0.
+        # Set kline_discontinuity_threshold to a large value if the unfolded kpoints line is continuous
+        # Unfold bandstructure
+        self._unfold_bandstructure(bandstructure, break_thresh=kline_discontinuity_threshold)
+        
+        # Save unfolded kpoints after post processing of wave function file
+        self._save_unfolded_kpts_bandstr(save_unfolded_kpts, save_unfolded_bandstr)
+        
+        return self.unfolded_bandstructure, self.kpline
```

### Comparing `banduppy-0.3.0/banduppy/unfolding.py` & `banduppy-0.3.1/banduppy/unfolding.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,585 +1,585 @@
-import numpy as np
-from .src import BandFolding, BandUnfolding
-from .Utilities import EBSplot, FoldingDegreePlot, BandCentersBroadening
-
-### ===========================================================================    
-class Unfolding(BandFolding, BandUnfolding, EBSplot, FoldingDegreePlot):
-    """
-    Band folding from primitive to supercell.
-
-    """
-    def __init__(self, supercell=None, print_log='low'):
-        """
-        Initialize the BandUPpy Unfolding class.
-
-        Parameters
-        ----------
-        supercell : 3X3 matrix, optional
-            Primitive-to-supercell transformation matrix. The default is Identity matrix.
-        print_log : [None,'low','medium','high'], optional
-            Print information of kpoints folding. Level of printing information. 
-            The default is 'low'. If None, nothing is printed.
-
-        """       
-        if print_log is not None: print_log = print_log.lower()
-        BandFolding.__init__(self, supercell=supercell, print_info=print_log)
-        
-    def propose_maximum_minimum_folding(self, pathPBZ, min_num_pts:int=5, max_num_pts:int=20,
-                                        serach_mode:str='brute_force', draw_plots:bool=True, 
-                                        save_plot:bool=False, save_dir='.', save_file_name=None,  
-                                        CountFig=None, yaxis_label:str='Folding degree (%)',
-                                        xaxis_label:str='number of kpoints', line_color='k'):
-        """
-        Calculates SC Kpoints from PC kpoints and returns percent of folding.
-        Maximum and Minimum degree of folding are reported.
-        
-        Folding percent = ((#of PC kpoints - #of folded SC Kpoints)/(#of PC kpoints))*100
-
-        Parameters
-        ----------
-        pathPBZ : ndarray/list
-            PC kpoint path nodes in reduced coordinates.
-        min_num_pts : int, optional
-            Minimum number of kpoints division in the k-path. The default is 5.
-        max_num_pts : int, optional
-            Maximum number of kpoints division in the k-path. The default is 20.
-        serach_mode : ['brute_force'], optional
-            Method to calculate SC Kpoints. The default is 'brute_force'.
-        draw_plots : bool, optional
-            Plot folding vs number of k-points. The default is True.
-            If True, also returns fig, ax, and CountFig.
-        save_plot : bool, optional
-            Save plots or not. The default is False.
-        save_dir : str/path, optional
-            Directory where to save the plots. The default is '.'.
-        save_file_name : str, optional
-            Name of the file to ba saved. The default is None. If None, figure
-            is not saved.
-        CountFig : int, optional
-            Figure count. The default is None. If None, nothing is is done. Else,
-            returns CountFig increased by 1.
-        yaxis_label : str, optional
-            yaxis label. The default is 'Folding degree (%)'.
-        xaxis_label : str, optional
-            xaxis label. The default is 'number of kpoints'.
-        line_color : matplotlib color, optional
-            Line color. The default is 'k'.
-
-        Returns
-        -------
-        proposed_folding_results : dictionary
-            {index: ((start node, end node), folding data)}
-            index : Index of path segment searched from the pathPBZ list supplied.
-            folding data : 2d array with each row containing number of division in the 1st
-            column and percent of folding in the 2nd column.
-            
-            If draw_plots=True, also returns fig, ax, and CountFig.
-        """
-        proposed_folding_results = \
-             self.propose_best_least_folding(pathPBZ, min_num_pts=min_num_pts, 
-                                             max_num_pts=max_num_pts,
-                                             serach_mode=serach_mode)
-        if draw_plots:
-            FoldingDegreePlot.__init__(self, fold_results_dictionary=proposed_folding_results, 
-                                       save_figure_dir=save_dir)
-            fig, ax, CountFig = self.plot_folding(save_file_name=save_file_name, 
-                                                  CountFig=CountFig, 
-                                                  yaxis_label=yaxis_label,
-                                                  xaxis_label=xaxis_label, 
-                                                  line_color=line_color)
-            return proposed_folding_results, fig, ax, CountFig
-        return proposed_folding_results
-        
-    def generate_SC_Kpts_from_pc_k_path(self, pathPBZ=None, nk=11, labels=None, kpts_weights=None, 
-                                        save_all_kpts:bool=False, save_sc_kpts:bool=False, 
-                                        save_dir='.', file_name:str='', 
-                                        file_name_suffix:str='', file_format:str='vasp'):
-        """
-        Generate supercell kpoints from reference primitive BZ k-path.
-
-        Parameters
-        ----------
-        pathPBZ : ndarray/list, optional
-            PC kpoint path nodes in reduced coordinates. 
-            If the segmant is skipped, put a None between nodes.
-            E.g. [[1/2,1/2,1/2], [0,0,0],None, [3/8,3/8,3/4], [0,0,0]] for [LGKG]
-            The default is None. 
-        nk : int ot tuple, optional
-            Number of kpoints in each k-path segment. The default is 11.
-            None in pathPBZ is not part of the segments. 
-            E.g. In [[1/2,1/2,1/2], [0,0,0],None, [3/8,3/8,3/4], [0,0,0]] there are
-            only 2 segments.
-        labels : string ot list of strings
-            Labels of special k-points, either as a continuous list or string. 
-            Do not use ',' or multidimentional list do define disjoint segmants.
-            e.g. Do not use labels='LG,KG'. Use labels='LGKG'. The 'None' in the
-            pathPBZ will take care of the disjoint segments.
-            If multiple word needs to be single label, use list.
-            e.g. labels=['X','Gamma','L']. Do not use string labels='XGammaL'.
-            The default is None. If None, the special
-            kpoints will be indexed as 1,2,3,...
-        kpts_weights : int or float or 1d numpy array, optional
-            Weights of the SC kpoints. The default is None. If none, no weights are padded
-            in the generated SC K-points list.
-        save_all_kpts : bool, optional
-            Save the PC kpoints, generated SC kpoints, and SC-PC kpoints mapping. 
-            The default is False. If True, has precedence over save_sc_kpts.
-        save_sc_kpts : bool, optional
-            Save the generated SC kpoints. The default is False.
-        save_dir : str/path_object, optional
-            Directory to save the file. The default is current directory.
-        file_name : str, optional
-            Name of the file. The default is ''.
-            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
-        file_name_suffix : str, optional
-            Suffix to add after the file_name. The default is ''.
-        file_format : ['vasp'], optional
-            Format of the file. The default is 'vasp'. 
-            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
-
-        Returns
-        -------
-        ndarray of floats
-            PC kpoints list.
-        ndarray of floats
-            SC kpoints list.
-        ndarray of int
-            PC unique kpoints indices for reverse engineer.
-        ndarray of int
-            SC unique kpoints indices for reverse engineer.
-
-        """
-        return self.generate_SC_K_from_pc_k_path(pathPBZ=pathPBZ, nk=nk, labels=labels, 
-                                                 kpts_weights=kpts_weights, 
-                                                 save_all_kpts=save_all_kpts, 
-                                                 save_sc_kpts=save_sc_kpts, 
-                                                 save_dir=save_dir, file_name=file_name, 
-                                                 file_name_suffix=file_name_suffix, 
-                                                 file_format=file_format)
-            
-    def generate_SC_Kpts_from_pc_kpts(self, kpointsPBZ=None, kpts_weights=None,
-                                      save_all_kpts:bool=False, save_sc_kpts:bool=False, 
-                                      save_dir='.', file_name:str='', 
-                                      file_name_suffix:str='', file_format:str='vasp', footer_msg=None,
-                                      special_kpoints_pos_labels=None):
-        """
-        Generate supercell kpoints from reference primitive kpoints.
-
-        Parameters
-        ----------
-        kpointsPBZ : ndarray, optional
-            PC kpoint list. The default is None. 
-        kpts_weights : int or float or 1d numpy array, optional
-            Weights of the SC kpoints. The default is None. If none, no weights are padded
-            in the generated SC K-points list.
-        save_all_kpts : bool, optional
-            Save the PC kpoints, generated SC kpoints, and SC-PC kpoints mapping. 
-            The default is False. If True, has precedence over save_sc_kpts.
-        save_sc_kpts : bool, optional
-            Save the generated SC kpoints. The default is False.
-        save_dir : str/path_object, optional
-            Directory to save the file. The default is current directory.
-        file_name : str, optional
-            Name of the file. The default is ''.
-            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
-        file_name_suffix : str, optional
-            Suffix to add after the file_name. The default is ''.
-        file_format : ['vasp'], optional
-            Format of the file. The default is 'vasp'. 
-            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
-        footer_msg : str, optional
-            String that will be written at the end of the file. The default is PC kpoints list.
-        special_kpoints_pos_labels : dictionary, optional
-            Special kpoints position_index in PC kpoints list as key and label as value. 
-            Will be used in plotting. Default is None.
-
-        Returns
-        -------
-        ndarray of floats
-            PC kpoints list (orginal provided k-path, full list).
-        ndarray of floats
-            PC kpoints list (unique).
-        ndarray of floats
-            SC kpoints list (unique).
-        dictionary of int/list
-            Mapping of SC kpts (K), PC unique kpts (k unique), and PC full kpts (k) indices.
-            format: {K index: K -> k index unique: k unique -> k index: k}
-            This mapping can be used for reverse engineer latter.
-        dictionary or None
-            Position and labels of special kpoints, will be used in plotting.
-
-        """
-        return self.generate_K_from_k(kpointsPBZ=kpointsPBZ, kpts_weights=kpts_weights,
-                                      save_all_kpts=save_all_kpts, 
-                                      save_sc_kpts=save_sc_kpts, 
-                                      save_dir=save_dir, file_name=file_name, 
-                                      file_name_suffix=file_name_suffix, 
-                                      file_format=file_format, footer_msg=footer_msg,
-                                      special_kpoints_pos_labels=special_kpoints_pos_labels)
-    
-    def Unfold(self, bandstructure,  
-               PBZ_kpts_list_full=None, SBZ_kpts_list=None, SBZ_PBZ_kpts_map=None,
-               kline_discontinuity_threshold = 0.1,
-               save_unfolded_kpts = {'save2file': False, 
-                                     'fdir': '.',
-                                     'fname': 'kpoints_unfolded',
-                                     'fname_suffix': ''},
-               save_unfolded_bandstr = {'save2file': False, 
-                                        'fdir': '.',
-                                        'fname': 'bandstructure_unfolded',
-                                        'fname_suffix': ''}):
-        """
-        Unfold the band structure.
-
-        Parameters
-        ----------
-        bandstructure : irrep.bandstructure.BandStructure
-            irrep.bandstructure.BandStructure.
-        PBZ_kpts_list_full : ndarray, optional
-            List of PC k-points. If None, try to find the list from class instance.
-            The default is None.
-        SBZ_kpts_list : ndarray, optional
-            List of SC K-points. If None, try to find the list from class instance.
-            The default is None.
-        SBZ_PBZ_kpts_map : dictionary, optional
-            Mapping of SC generated K-points indices and PC k-points indices. 
-            If None, try to find the list from class instance.
-            The default is None.
-        kline_discontinuity_threshold : float, optional
-            If the distance between two neighboring k-points in the path is 
-            larger than `break_thresh` break continuity in k-path. Set break_thresh 
-            to a large value if the unfolded kpoints line is continuous.
-            The default is 0.1.
-        save_unfolded_kpts : dictionary, optional
-            save2file :: Save unfolded kpoints or not? 
-            fir :: str or path
-                Directory path where to save the file.
-            fname :: str
-                Name of the file.
-            fname_suffix :: str
-                Suffix to add to the file name.
-            The default is {'save2file': False, 'fdir': '.', 'fname': 'kpoints_unfolded', 'fname_suffix': ''}.
-        save_unfolded_bandstr : dictionary, optional
-            save2file :: Save unfolded kpoints or not? 
-            fir :: str or path
-                Directory path where to save the file.
-            fname :: str
-                Name of the file.
-            fname_suffix :: str
-                Suffix to add to the file name. 
-            The default is {'save2file': False, 'fdir': '.', 'fname': 'bandstructure_unfolded', 'fname_suffix': ''}.
-            
-        Returns
-        -------
-        numpy ndarray
-            Unfolded effective band structure. 
-            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
-        numpy ndarray
-            Unfolded effective band structure k-path.
-            Format: k on path (A^-1)
-
-        """
-        if (PBZ_kpts_list_full is None) or \
-            (SBZ_kpts_list in None) or (SBZ_PBZ_kpts_map is None):
-            BandUnfolding.__init__(self, self.transformation_matrix, 
-                                   self.PBZ_kpts_list_org, self.SBZ_kpts_list, 
-                                   self.SBZ_PBZ_kpts_mapping,
-                                   print_info=self.print_information)
-        else:
-            BandUnfolding.__init__(self, self.transformation_matrix, 
-                                   PBZ_kpts_list_full, SBZ_kpts_list, 
-                                   SBZ_PBZ_kpts_map, 
-                                   print_info=self.print_information)
-        
-        return self.unfold(bandstructure, 
-                           kline_discontinuity_threshold = kline_discontinuity_threshold,
-                           save_unfolded_kpts = save_unfolded_kpts,
-                           save_unfolded_bandstr = save_unfolded_bandstr)
-    
-    def plot_ebs(self, ax=None, save_figure_dir='.', save_file_name=None, CountFig=None, 
-                 Ef=None, Emin=None, Emax=None, pad_energy_scale:float=0.5, 
-                 threshold_weight:float=None, mode:str="fatband", 
-                 yaxis_label:str='E (eV)', special_kpoints:dict=None, plotSC:bool=True,  
-                 marker='o', fatfactor=20, nE:int=100, smear:float=0.05, 
-                 scatter_color='gray', color_map='viridis', show_legend:bool=True):
-        """
-        Scatter/density plot of the band structure.
-
-        Parameters
-        ----------
-        ax : matplotlib.pyplot axis, optional
-            Figure axis to plot on. If None, new figure will be created.
-            The default is None.
-        save_figure_dir : str, optional
-            Directory where to save the figure. The default is current directory.
-        save_file_name : str, optional
-            Name of the figure file. If None, figure will be not saved. 
-            The default is None.
-        CountFig: int, optional
-            Figure count. The default is None.
-        Ef : float, optional
-            Fermi energy. If None, set to 0.0. The default is None.
-        Emin : float, optional
-            Minimum in energy. The default is None.
-        Emax : float, optional
-            Maximum in energy. The default is None.
-        pad_energy_scale: float, optional
-            Add padding of pad_energy_scale to minimum and maximum energy if Emin
-            and Emax are None. The default is 0.5.
-        threshold_weight : float, optional
-            The band centers with band weights lower than the threshhold weights 
-            are discarded. The default is None. If None, this is ignored.
-        mode : ['fatband','density'], optional
-            Mode of plot. The default is "fatband".
-        yaxis_label : str, optional
-            Y-axis label text. The default is 'E (eV)'.
-        special_kpoints : dictionary, optional
-            Dictionary of special kpoints position and labels. If None, ignore
-            special kpoints. The default is None.
-        plotSC : bool, optional
-            Plot supercell bandstructure. The default is True.
-        marker : matplotlib.pyplot markerMarkerStyle, optional
-            The marker style. Marker can be either an instance of the class or 
-            the text shorthand for a particular marker. 
-            The default is 'o'.
-        fatfactor : int, optional
-            Scatter plot marker size. The default is 20.
-        nE : int, optional
-            Number of pixels in Energy scale when used 'density' mode. 
-            The default is 100.
-        smear : float, optional
-            Gaussian smearing. The default is 0.05.
-        scatter_color : str/color, optional
-            Color of scatter plot of unfolded band structure. The color of supercell
-            band structures is gray. The default is 'gray'.
-        color_map: str/ matplotlib colormap
-            Colormap for density plot. The default is viridis.
-        show_legend : bool
-            If show legend or not. The default is True.
-
-        Returns
-        -------
-        fig : matplotlib.pyplot.figure
-            Figure instance. If ax is not None previously generated fig instance
-            will be used.
-        ax : Axis instance
-            Figure axis instance.
-        CountFig: int or None
-            Figure count.
-
-        """
-        
-        EBSplot.__init__(self, save_figure_dir=save_figure_dir)
-
-        return self.plot(ax=ax, save_file_name=save_file_name, CountFig=CountFig, Ef=Ef, 
-                         Emin=Emin, Emax=Emax, pad_energy_scale=pad_energy_scale, 
-                         threshold_weight=threshold_weight, mode=mode,
-                         yaxis_label=yaxis_label, special_kpoints=special_kpoints, 
-                         plotSC=plotSC, marker=marker, fatfactor=fatfactor, nE=nE, 
-                         smear=smear, scatter_color=scatter_color, color_map=color_map,
-                         show_legend=show_legend)
-    
-class Properties(BandCentersBroadening):
-    """
-    Calculate properties from unfolded band structure.
-
-    """
-    def __init__(self, print_log='low'):
-        """
-        Initialize the BandUPpy Properties class.
-
-        Parameters
-        ----------
-        print_log : [None,'low','medium','high'], optional
-            Print information of kpoints folding. Level of printing information. 
-            The default is 'low'. If None, nothing is printed.
-
-        """       
-        if print_log is not None: self.print_log_info = print_log.lower()
-    
-    def band_centers_broadening_bandstr(self, unfolded_bandstructure, 
-                                        min_dN_pre_screening:float=1e-4,
-                                        threshold_dN_2b_trial_band_center:float=0.05,
-                                        min_sum_dNs_for_a_band:float=0.05, 
-                                        precision_pos_band_centers:float=1e-5,
-                                        err_tolerance_compare_kpts:float=1e-8,
-                                        collect_scf_data:bool=False,
-                                        save_data = {'save2file': False, 
-                                                     'fdir': '.',
-                                                     'fname': 'unfolded_bandcenters',
-                                                     'fname_suffix': ''}):
-        """
-        Find band centers and broadening of the unfolded band structure.
-
-        Parameters
-        ----------
-        unfolded_bandstructure : numpy array
-            Unfolded effective band structure. 
-            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
-        min_dN_pre_screening : float, optional
-            Discard the bands which has weights below min_dN_pre_screening. This
-            pre-screening step helps to minimize the data that will processed
-            now on. The default is 1e-4.
-        threshold_dN_2b_trial_band_center : float, optional
-            Initial guess of the band centers based on the threshold wights.
-            The default is 0.05.
-        min_sum_dNs_for_a_band : float, optional
-            Cut off criteria for minimum weights that band center should have. 
-            The band centers with lower weights than min_sum_dNs_for_a_band will be
-            discarded during SCF refinements. If min_sum_dNs_for_a_band  
-            is smaller than threshold_dN_2b_trial_band_center, min_sum_dNs_for_a_band
-            will be reset to threshold_dN_2b_trial_band_center value.
-            The default is 0.05.
-        precision_pos_band_centers : float, optional
-            Precision when compared band centers from previous and latest SCF
-            iteration. SCF is considered converged if this precision is reached.
-            The default is 1e-5.
-        err_tolerance_compare_kpts : float, optional
-            The tolerance to group the bands set per unique kpoints.
-            The default is 1e-8.
-        collect_scf_data : bool, optional
-            Whether to save the dtails of band centers in each SCF cycles.
-            The default is False.
-        save_data : dictionary, optional
-            save2file :: Save unfolded kpoints or not? 
-            fir :: str or path
-                Directory path where to save the file.
-            fname :: str
-                Name of the file.
-            fname_suffix :: str
-                Suffix to add to the file name.
-            The default is {'save2file': False, 'fdir': '.', 'fname': 'unfolded_bandcenters', 'fname_suffix': ''}.
-
-        Returns
-        -------
-        list of array
-            Each array contains the final details of band centers in a particular
-            kpoint. The list contains band center details for each kpoints.
-            Format: kpoint coordinate, Band center, Band width, Sum of dN.
-        dictionary of dictionary of array or None
-            Each array contains the final details of band centers in a particular
-            kpoint. The dictionary then contains the details for each SCF cycles with
-            keys are the SCF cycle number. The highest level dictionary then contains 
-            details for each kpoints with keys are the kpoint indices. Returns None
-            if collect_scf_data is false.
-
-        """
-        BandCentersBroadening.__init__(self, unfolded_bandstructure=unfolded_bandstructure, 
-                                       min_dN_pre_screening=min_dN_pre_screening,
-                                       threshold_dN_2b_trial_band_center=threshold_dN_2b_trial_band_center,
-                                       min_sum_dNs_for_a_band=min_sum_dNs_for_a_band, 
-                                       precision_pos_band_centers=precision_pos_band_centers,
-                                       err_tolerance_compare_kpts=err_tolerance_compare_kpts,
-                                       print_log=self.print_log_info)
-        return self.scfs_band_centers_broadening(collect_data_scf=collect_scf_data,
-                                                 save_data=save_data)
-
-class Plotting(EBSplot):
-    
-    def __init__(self, save_figure_dir='.'):
-        """
-        Intializing BandUPpy Plotting class.
-
-        Parameters
-        ----------
-        save_figure_dir : str, optional
-            Directory where to save the figure. The default is current directory.
-
-        """
-        self.save_figure_directory = save_figure_dir
-    
-    def plot_ebs(self, kpath_in_angs, unfolded_bandstructure, 
-                 ax=None, save_file_name=None, CountFig=None, 
-                 Ef=None, Emin=None, Emax=None, pad_energy_scale:float=0.5, 
-                 threshold_weight:float=None, mode:str="fatband", 
-                 yaxis_label:str='E (eV)', special_kpoints:dict=None, plotSC:bool=True,  
-                 marker='o', fatfactor=20, nE:int=100, smear:float=0.05, 
-                 color='gray', color_map='viridis', show_legend:bool=True,
-                 plot_colormap_bandcenter:bool=True):
-        """
-        Scatter/density/band_centers plot of the band structure.
-
-        Parameters
-        ----------
-        kpath_in_angs : array, optional
-            k on path (in A^-1) coordinate. The default is None.
-        unfolded_bandstructure : ndarray, optional
-            Unfolded effective band structure data. 
-            Format: k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
-            The default is None.
-        ax : matplotlib.pyplot axis, optional
-            Figure axis to plot on. If None, new figure will be created.
-            The default is None.
-        save_file_name : str, optional
-            Name of the figure file. If None, figure will be not saved. 
-            The default is None.
-        CountFig: int, optional
-            Figure count. The default is None.
-        Ef : float, optional
-            Fermi energy. If None, set to 0.0. The default is None.
-        Emin : float, optional
-            Minimum in energy. The default is None.
-        Emax : float, optional
-            Maximum in energy. The default is None.
-        pad_energy_scale: float, optional
-            Add padding of pad_energy_scale to minimum and maximum energy if Emin
-            and Emax are None. The default is 0.5.
-        threshold_weight : float, optional
-            The band centers with band weights lower than the threshhold weights 
-            are discarded. The default is None. If None, this is ignored.
-        mode : ['fatband','density', 'band_centers'], optional
-            Mode of plot. The default is "fatband".
-        yaxis_label : str, optional
-            Y-axis label text. The default is 'E (eV)'.
-        special_kpoints : dictionary, optional
-            Dictionary of special kpoints position and labels. If None, ignore
-            special kpoints. The default is None.
-        plotSC : bool, optional
-            Plot supercell bandstructure. The default is True.
-        marker : matplotlib.pyplot markerMarkerStyle, optional
-            The marker style. Marker can be either an instance of the class or 
-            the text shorthand for a particular marker. 
-            The default is 'o'.
-        fatfactor : int, optional
-            Scatter plot marker size. The default is 20.
-        nE : int, optional
-            Number of pixels in Energy scale when used 'density' mode. 
-            The default is 100.
-        smear : float, optional
-            Gaussian smearing. The default is 0.05.
-        color : str/color, optional
-            Color of plot of unfolded band structure. The color of supercell
-            band structures is gray. The default is 'gray'.
-        color_map: str/ matplotlib colormap
-            Colormap for density plot. The default is viridis.
-        show_legend : bool
-            If show legend or not. The default is True.
-        plot_colormap_bandcenter : bool, optional
-            If plotting the band ceneters by colormap. The default is True.
-
-        Returns
-        -------
-        fig : matplotlib.pyplot.figure
-            Figure instance. If ax is not None previously generated fig instance
-            will be used.
-        ax : Axis instance
-            Figure axis instance.
-        CountFig: int or None
-            Figure count.
-
-        """
-        
-        EBSplot.__init__(self, kpath_in_angs=kpath_in_angs, 
-                         unfolded_bandstructure=unfolded_bandstructure, 
-                         save_figure_dir=self.save_figure_directory)
-
-        return self.plot(ax=ax, save_file_name=save_file_name, CountFig=CountFig, Ef=Ef, 
-                         Emin=Emin, Emax=Emax, pad_energy_scale=pad_energy_scale, 
-                         threshold_weight=threshold_weight, mode=mode,
-                         yaxis_label=yaxis_label, special_kpoints=special_kpoints, 
-                         plotSC=plotSC, marker=marker, fatfactor=fatfactor, nE=nE, 
-                         smear=smear, color=color, color_map=color_map,
-                         plot_colormap_bandcenter=plot_colormap_bandcenter,
-                         show_legend=show_legend)
-        
-
+import numpy as np
+from .src import BandFolding, BandUnfolding
+from .Utilities import EBSplot, FoldingDegreePlot, BandCentersBroadening
+
+### ===========================================================================    
+class Unfolding(BandFolding, BandUnfolding, EBSplot, FoldingDegreePlot):
+    """
+    Band folding from primitive to supercell.
+
+    """
+    def __init__(self, supercell=None, print_log='low'):
+        """
+        Initialize the BandUPpy Unfolding class.
+
+        Parameters
+        ----------
+        supercell : 3X3 matrix, optional
+            Primitive-to-supercell transformation matrix. The default is Identity matrix.
+        print_log : [None,'low','medium','high'], optional
+            Print information of kpoints folding. Level of printing information. 
+            The default is 'low'. If None, nothing is printed.
+
+        """       
+        if print_log is not None: print_log = print_log.lower()
+        BandFolding.__init__(self, supercell=supercell, print_info=print_log)
+        
+    def propose_maximum_minimum_folding(self, pathPBZ, min_num_pts:int=5, max_num_pts:int=20,
+                                        serach_mode:str='brute_force', draw_plots:bool=True, 
+                                        save_plot:bool=False, save_dir='.', save_file_name=None,  
+                                        CountFig=None, yaxis_label:str='Folding degree (%)',
+                                        xaxis_label:str='number of kpoints', line_color='k'):
+        """
+        Calculates SC Kpoints from PC kpoints and returns percent of folding.
+        Maximum and Minimum degree of folding are reported.
+        
+        Folding percent = ((#of PC kpoints - #of folded SC Kpoints)/(#of PC kpoints))*100
+
+        Parameters
+        ----------
+        pathPBZ : ndarray/list
+            PC kpoint path nodes in reduced coordinates.
+        min_num_pts : int, optional
+            Minimum number of kpoints division in the k-path. The default is 5.
+        max_num_pts : int, optional
+            Maximum number of kpoints division in the k-path. The default is 20.
+        serach_mode : ['brute_force'], optional
+            Method to calculate SC Kpoints. The default is 'brute_force'.
+        draw_plots : bool, optional
+            Plot folding vs number of k-points. The default is True.
+            If True, also returns fig, ax, and CountFig.
+        save_plot : bool, optional
+            Save plots or not. The default is False.
+        save_dir : str/path, optional
+            Directory where to save the plots. The default is '.'.
+        save_file_name : str, optional
+            Name of the file to ba saved. The default is None. If None, figure
+            is not saved.
+        CountFig : int, optional
+            Figure count. The default is None. If None, nothing is is done. Else,
+            returns CountFig increased by 1.
+        yaxis_label : str, optional
+            yaxis label. The default is 'Folding degree (%)'.
+        xaxis_label : str, optional
+            xaxis label. The default is 'number of kpoints'.
+        line_color : matplotlib color, optional
+            Line color. The default is 'k'.
+
+        Returns
+        -------
+        proposed_folding_results : dictionary
+            {index: ((start node, end node), folding data)}
+            index : Index of path segment searched from the pathPBZ list supplied.
+            folding data : 2d array with each row containing number of division in the 1st
+            column and percent of folding in the 2nd column.
+            
+            If draw_plots=True, also returns fig, ax, and CountFig.
+        """
+        proposed_folding_results = \
+             self.propose_best_least_folding(pathPBZ, min_num_pts=min_num_pts, 
+                                             max_num_pts=max_num_pts,
+                                             serach_mode=serach_mode)
+        if draw_plots:
+            FoldingDegreePlot.__init__(self, fold_results_dictionary=proposed_folding_results, 
+                                       save_figure_dir=save_dir)
+            fig, ax, CountFig = self.plot_folding(save_file_name=save_file_name, 
+                                                  CountFig=CountFig, 
+                                                  yaxis_label=yaxis_label,
+                                                  xaxis_label=xaxis_label, 
+                                                  line_color=line_color)
+            return proposed_folding_results, fig, ax, CountFig
+        return proposed_folding_results
+        
+    def generate_SC_Kpts_from_pc_k_path(self, pathPBZ=None, nk=11, labels=None, kpts_weights=None, 
+                                        save_all_kpts:bool=False, save_sc_kpts:bool=False, 
+                                        save_dir='.', file_name:str='', 
+                                        file_name_suffix:str='', file_format:str='vasp'):
+        """
+        Generate supercell kpoints from reference primitive BZ k-path.
+
+        Parameters
+        ----------
+        pathPBZ : ndarray/list, optional
+            PC kpoint path nodes in reduced coordinates. 
+            If the segmant is skipped, put a None between nodes.
+            E.g. [[1/2,1/2,1/2], [0,0,0],None, [3/8,3/8,3/4], [0,0,0]] for [LGKG]
+            The default is None. 
+        nk : int ot tuple, optional
+            Number of kpoints in each k-path segment. The default is 11.
+            None in pathPBZ is not part of the segments. 
+            E.g. In [[1/2,1/2,1/2], [0,0,0],None, [3/8,3/8,3/4], [0,0,0]] there are
+            only 2 segments.
+        labels : string ot list of strings
+            Labels of special k-points, either as a continuous list or string. 
+            Do not use ',' or multidimentional list do define disjoint segmants.
+            e.g. Do not use labels='LG,KG'. Use labels='LGKG'. The 'None' in the
+            pathPBZ will take care of the disjoint segments.
+            If multiple word needs to be single label, use list.
+            e.g. labels=['X','Gamma','L']. Do not use string labels='XGammaL'.
+            The default is None. If None, the special
+            kpoints will be indexed as 1,2,3,...
+        kpts_weights : int or float or 1d numpy array, optional
+            Weights of the SC kpoints. The default is None. If none, no weights are padded
+            in the generated SC K-points list.
+        save_all_kpts : bool, optional
+            Save the PC kpoints, generated SC kpoints, and SC-PC kpoints mapping. 
+            The default is False. If True, has precedence over save_sc_kpts.
+        save_sc_kpts : bool, optional
+            Save the generated SC kpoints. The default is False.
+        save_dir : str/path_object, optional
+            Directory to save the file. The default is current directory.
+        file_name : str, optional
+            Name of the file. The default is ''.
+            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
+        file_name_suffix : str, optional
+            Suffix to add after the file_name. The default is ''.
+        file_format : ['vasp'], optional
+            Format of the file. The default is 'vasp'. 
+            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
+
+        Returns
+        -------
+        ndarray of floats
+            PC kpoints list.
+        ndarray of floats
+            SC kpoints list.
+        ndarray of int
+            PC unique kpoints indices for reverse engineer.
+        ndarray of int
+            SC unique kpoints indices for reverse engineer.
+
+        """
+        return self.generate_SC_K_from_pc_k_path(pathPBZ=pathPBZ, nk=nk, labels=labels, 
+                                                 kpts_weights=kpts_weights, 
+                                                 save_all_kpts=save_all_kpts, 
+                                                 save_sc_kpts=save_sc_kpts, 
+                                                 save_dir=save_dir, file_name=file_name, 
+                                                 file_name_suffix=file_name_suffix, 
+                                                 file_format=file_format)
+            
+    def generate_SC_Kpts_from_pc_kpts(self, kpointsPBZ=None, kpts_weights=None,
+                                      save_all_kpts:bool=False, save_sc_kpts:bool=False, 
+                                      save_dir='.', file_name:str='', 
+                                      file_name_suffix:str='', file_format:str='vasp', footer_msg=None,
+                                      special_kpoints_pos_labels=None):
+        """
+        Generate supercell kpoints from reference primitive kpoints.
+
+        Parameters
+        ----------
+        kpointsPBZ : ndarray, optional
+            PC kpoint list. The default is None. 
+        kpts_weights : int or float or 1d numpy array, optional
+            Weights of the SC kpoints. The default is None. If none, no weights are padded
+            in the generated SC K-points list.
+        save_all_kpts : bool, optional
+            Save the PC kpoints, generated SC kpoints, and SC-PC kpoints mapping. 
+            The default is False. If True, has precedence over save_sc_kpts.
+        save_sc_kpts : bool, optional
+            Save the generated SC kpoints. The default is False.
+        save_dir : str/path_object, optional
+            Directory to save the file. The default is current directory.
+        file_name : str, optional
+            Name of the file. The default is ''.
+            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
+        file_name_suffix : str, optional
+            Suffix to add after the file_name. The default is ''.
+        file_format : ['vasp'], optional
+            Format of the file. The default is 'vasp'. 
+            If file_format is vasp, file_name=KPOINTS_<file_name_suffix>
+        footer_msg : str, optional
+            String that will be written at the end of the file. The default is PC kpoints list.
+        special_kpoints_pos_labels : dictionary, optional
+            Special kpoints position_index in PC kpoints list as key and label as value. 
+            Will be used in plotting. Default is None.
+
+        Returns
+        -------
+        ndarray of floats
+            PC kpoints list (orginal provided k-path, full list).
+        ndarray of floats
+            PC kpoints list (unique).
+        ndarray of floats
+            SC kpoints list (unique).
+        dictionary of int/list
+            Mapping of SC kpts (K), PC unique kpts (k unique), and PC full kpts (k) indices.
+            format: {K index: K -> k index unique: k unique -> k index: k}
+            This mapping can be used for reverse engineer latter.
+        dictionary or None
+            Position and labels of special kpoints, will be used in plotting.
+
+        """
+        return self.generate_K_from_k(kpointsPBZ=kpointsPBZ, kpts_weights=kpts_weights,
+                                      save_all_kpts=save_all_kpts, 
+                                      save_sc_kpts=save_sc_kpts, 
+                                      save_dir=save_dir, file_name=file_name, 
+                                      file_name_suffix=file_name_suffix, 
+                                      file_format=file_format, footer_msg=footer_msg,
+                                      special_kpoints_pos_labels=special_kpoints_pos_labels)
+    
+    def Unfold(self, bandstructure,  
+               PBZ_kpts_list_full=None, SBZ_kpts_list=None, SBZ_PBZ_kpts_map=None,
+               kline_discontinuity_threshold = 0.1,
+               save_unfolded_kpts = {'save2file': False, 
+                                     'fdir': '.',
+                                     'fname': 'kpoints_unfolded',
+                                     'fname_suffix': ''},
+               save_unfolded_bandstr = {'save2file': False, 
+                                        'fdir': '.',
+                                        'fname': 'bandstructure_unfolded',
+                                        'fname_suffix': ''}):
+        """
+        Unfold the band structure.
+
+        Parameters
+        ----------
+        bandstructure : irrep.bandstructure.BandStructure
+            irrep.bandstructure.BandStructure.
+        PBZ_kpts_list_full : ndarray, optional
+            List of PC k-points. If None, try to find the list from class instance.
+            The default is None.
+        SBZ_kpts_list : ndarray, optional
+            List of SC K-points. If None, try to find the list from class instance.
+            The default is None.
+        SBZ_PBZ_kpts_map : dictionary, optional
+            Mapping of SC generated K-points indices and PC k-points indices. 
+            If None, try to find the list from class instance.
+            The default is None.
+        kline_discontinuity_threshold : float, optional
+            If the distance between two neighboring k-points in the path is 
+            larger than `break_thresh` break continuity in k-path. Set break_thresh 
+            to a large value if the unfolded kpoints line is continuous.
+            The default is 0.1.
+        save_unfolded_kpts : dictionary, optional
+            save2file :: Save unfolded kpoints or not? 
+            fir :: str or path
+                Directory path where to save the file.
+            fname :: str
+                Name of the file.
+            fname_suffix :: str
+                Suffix to add to the file name.
+            The default is {'save2file': False, 'fdir': '.', 'fname': 'kpoints_unfolded', 'fname_suffix': ''}.
+        save_unfolded_bandstr : dictionary, optional
+            save2file :: Save unfolded kpoints or not? 
+            fir :: str or path
+                Directory path where to save the file.
+            fname :: str
+                Name of the file.
+            fname_suffix :: str
+                Suffix to add to the file name. 
+            The default is {'save2file': False, 'fdir': '.', 'fname': 'bandstructure_unfolded', 'fname_suffix': ''}.
+            
+        Returns
+        -------
+        numpy ndarray
+            Unfolded effective band structure. 
+            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
+        numpy ndarray
+            Unfolded effective band structure k-path.
+            Format: k on path (A^-1)
+
+        """
+        if (PBZ_kpts_list_full is None) or \
+            (SBZ_kpts_list in None) or (SBZ_PBZ_kpts_map is None):
+            BandUnfolding.__init__(self, self.transformation_matrix, 
+                                   self.PBZ_kpts_list_org, self.SBZ_kpts_list, 
+                                   self.SBZ_PBZ_kpts_mapping,
+                                   print_info=self.print_information)
+        else:
+            BandUnfolding.__init__(self, self.transformation_matrix, 
+                                   PBZ_kpts_list_full, SBZ_kpts_list, 
+                                   SBZ_PBZ_kpts_map, 
+                                   print_info=self.print_information)
+        
+        return self.unfold(bandstructure, 
+                           kline_discontinuity_threshold = kline_discontinuity_threshold,
+                           save_unfolded_kpts = save_unfolded_kpts,
+                           save_unfolded_bandstr = save_unfolded_bandstr)
+    
+    def plot_ebs(self, ax=None, save_figure_dir='.', save_file_name=None, CountFig=None, 
+                 Ef=None, Emin=None, Emax=None, pad_energy_scale:float=0.5, 
+                 threshold_weight:float=None, mode:str="fatband", 
+                 yaxis_label:str='E (eV)', special_kpoints:dict=None, plotSC:bool=True,  
+                 marker='o', fatfactor=20, nE:int=100, smear:float=0.05, 
+                 scatter_color='gray', color_map='viridis', show_legend:bool=True):
+        """
+        Scatter/density plot of the band structure.
+
+        Parameters
+        ----------
+        ax : matplotlib.pyplot axis, optional
+            Figure axis to plot on. If None, new figure will be created.
+            The default is None.
+        save_figure_dir : str, optional
+            Directory where to save the figure. The default is current directory.
+        save_file_name : str, optional
+            Name of the figure file. If None, figure will be not saved. 
+            The default is None.
+        CountFig: int, optional
+            Figure count. The default is None.
+        Ef : float, optional
+            Fermi energy. If None, set to 0.0. The default is None.
+        Emin : float, optional
+            Minimum in energy. The default is None.
+        Emax : float, optional
+            Maximum in energy. The default is None.
+        pad_energy_scale: float, optional
+            Add padding of pad_energy_scale to minimum and maximum energy if Emin
+            and Emax are None. The default is 0.5.
+        threshold_weight : float, optional
+            The band centers with band weights lower than the threshhold weights 
+            are discarded. The default is None. If None, this is ignored.
+        mode : ['fatband','density'], optional
+            Mode of plot. The default is "fatband".
+        yaxis_label : str, optional
+            Y-axis label text. The default is 'E (eV)'.
+        special_kpoints : dictionary, optional
+            Dictionary of special kpoints position and labels. If None, ignore
+            special kpoints. The default is None.
+        plotSC : bool, optional
+            Plot supercell bandstructure. The default is True.
+        marker : matplotlib.pyplot markerMarkerStyle, optional
+            The marker style. Marker can be either an instance of the class or 
+            the text shorthand for a particular marker. 
+            The default is 'o'.
+        fatfactor : int, optional
+            Scatter plot marker size. The default is 20.
+        nE : int, optional
+            Number of pixels in Energy scale when used 'density' mode. 
+            The default is 100.
+        smear : float, optional
+            Gaussian smearing. The default is 0.05.
+        scatter_color : str/color, optional
+            Color of scatter plot of unfolded band structure. The color of supercell
+            band structures is gray. The default is 'gray'.
+        color_map: str/ matplotlib colormap
+            Colormap for density plot. The default is viridis.
+        show_legend : bool
+            If show legend or not. The default is True.
+
+        Returns
+        -------
+        fig : matplotlib.pyplot.figure
+            Figure instance. If ax is not None previously generated fig instance
+            will be used.
+        ax : Axis instance
+            Figure axis instance.
+        CountFig: int or None
+            Figure count.
+
+        """
+        
+        EBSplot.__init__(self, save_figure_dir=save_figure_dir)
+
+        return self.plot(ax=ax, save_file_name=save_file_name, CountFig=CountFig, Ef=Ef, 
+                         Emin=Emin, Emax=Emax, pad_energy_scale=pad_energy_scale, 
+                         threshold_weight=threshold_weight, mode=mode,
+                         yaxis_label=yaxis_label, special_kpoints=special_kpoints, 
+                         plotSC=plotSC, marker=marker, fatfactor=fatfactor, nE=nE, 
+                         smear=smear, scatter_color=scatter_color, color_map=color_map,
+                         show_legend=show_legend)
+    
+class Properties(BandCentersBroadening):
+    """
+    Calculate properties from unfolded band structure.
+
+    """
+    def __init__(self, print_log='low'):
+        """
+        Initialize the BandUPpy Properties class.
+
+        Parameters
+        ----------
+        print_log : [None,'low','medium','high'], optional
+            Print information of kpoints folding. Level of printing information. 
+            The default is 'low'. If None, nothing is printed.
+
+        """       
+        if print_log is not None: self.print_log_info = print_log.lower()
+    
+    def band_centers_broadening_bandstr(self, unfolded_bandstructure, 
+                                        min_dN_pre_screening:float=1e-4,
+                                        threshold_dN_2b_trial_band_center:float=0.05,
+                                        min_sum_dNs_for_a_band:float=0.05, 
+                                        precision_pos_band_centers:float=1e-5,
+                                        err_tolerance_compare_kpts:float=1e-8,
+                                        collect_scf_data:bool=False,
+                                        save_data = {'save2file': False, 
+                                                     'fdir': '.',
+                                                     'fname': 'unfolded_bandcenters',
+                                                     'fname_suffix': ''}):
+        """
+        Find band centers and broadening of the unfolded band structure.
+
+        Parameters
+        ----------
+        unfolded_bandstructure : numpy array
+            Unfolded effective band structure. 
+            Format: k index, k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
+        min_dN_pre_screening : float, optional
+            Discard the bands which has weights below min_dN_pre_screening. This
+            pre-screening step helps to minimize the data that will processed
+            now on. The default is 1e-4.
+        threshold_dN_2b_trial_band_center : float, optional
+            Initial guess of the band centers based on the threshold wights.
+            The default is 0.05.
+        min_sum_dNs_for_a_band : float, optional
+            Cut off criteria for minimum weights that band center should have. 
+            The band centers with lower weights than min_sum_dNs_for_a_band will be
+            discarded during SCF refinements. If min_sum_dNs_for_a_band  
+            is smaller than threshold_dN_2b_trial_band_center, min_sum_dNs_for_a_band
+            will be reset to threshold_dN_2b_trial_band_center value.
+            The default is 0.05.
+        precision_pos_band_centers : float, optional
+            Precision when compared band centers from previous and latest SCF
+            iteration. SCF is considered converged if this precision is reached.
+            The default is 1e-5.
+        err_tolerance_compare_kpts : float, optional
+            The tolerance to group the bands set per unique kpoints.
+            The default is 1e-8.
+        collect_scf_data : bool, optional
+            Whether to save the dtails of band centers in each SCF cycles.
+            The default is False.
+        save_data : dictionary, optional
+            save2file :: Save unfolded kpoints or not? 
+            fir :: str or path
+                Directory path where to save the file.
+            fname :: str
+                Name of the file.
+            fname_suffix :: str
+                Suffix to add to the file name.
+            The default is {'save2file': False, 'fdir': '.', 'fname': 'unfolded_bandcenters', 'fname_suffix': ''}.
+
+        Returns
+        -------
+        list of array
+            Each array contains the final details of band centers in a particular
+            kpoint. The list contains band center details for each kpoints.
+            Format: kpoint coordinate, Band center, Band width, Sum of dN.
+        dictionary of dictionary of array or None
+            Each array contains the final details of band centers in a particular
+            kpoint. The dictionary then contains the details for each SCF cycles with
+            keys are the SCF cycle number. The highest level dictionary then contains 
+            details for each kpoints with keys are the kpoint indices. Returns None
+            if collect_scf_data is false.
+
+        """
+        BandCentersBroadening.__init__(self, unfolded_bandstructure=unfolded_bandstructure, 
+                                       min_dN_pre_screening=min_dN_pre_screening,
+                                       threshold_dN_2b_trial_band_center=threshold_dN_2b_trial_band_center,
+                                       min_sum_dNs_for_a_band=min_sum_dNs_for_a_band, 
+                                       precision_pos_band_centers=precision_pos_band_centers,
+                                       err_tolerance_compare_kpts=err_tolerance_compare_kpts,
+                                       print_log=self.print_log_info)
+        return self.scfs_band_centers_broadening(collect_data_scf=collect_scf_data,
+                                                 save_data=save_data)
+
+class Plotting(EBSplot):
+    
+    def __init__(self, save_figure_dir='.'):
+        """
+        Intializing BandUPpy Plotting class.
+
+        Parameters
+        ----------
+        save_figure_dir : str, optional
+            Directory where to save the figure. The default is current directory.
+
+        """
+        self.save_figure_directory = save_figure_dir
+    
+    def plot_ebs(self, kpath_in_angs, unfolded_bandstructure, 
+                 ax=None, save_file_name=None, CountFig=None, 
+                 Ef=None, Emin=None, Emax=None, pad_energy_scale:float=0.5, 
+                 threshold_weight:float=None, mode:str="fatband", 
+                 yaxis_label:str='E (eV)', special_kpoints:dict=None, plotSC:bool=True,  
+                 marker='o', fatfactor=20, nE:int=100, smear:float=0.05, 
+                 color='gray', color_map='viridis', show_legend:bool=True,
+                 plot_colormap_bandcenter:bool=True):
+        """
+        Scatter/density/band_centers plot of the band structure.
+
+        Parameters
+        ----------
+        kpath_in_angs : array, optional
+            k on path (in A^-1) coordinate. The default is None.
+        unfolded_bandstructure : ndarray, optional
+            Unfolded effective band structure data. 
+            Format: k on path (A^-1), energy, weight, "Sx, Sy, Sz" if is_spinor.
+            The default is None.
+        ax : matplotlib.pyplot axis, optional
+            Figure axis to plot on. If None, new figure will be created.
+            The default is None.
+        save_file_name : str, optional
+            Name of the figure file. If None, figure will be not saved. 
+            The default is None.
+        CountFig: int, optional
+            Figure count. The default is None.
+        Ef : float, optional
+            Fermi energy. If None, set to 0.0. The default is None.
+        Emin : float, optional
+            Minimum in energy. The default is None.
+        Emax : float, optional
+            Maximum in energy. The default is None.
+        pad_energy_scale: float, optional
+            Add padding of pad_energy_scale to minimum and maximum energy if Emin
+            and Emax are None. The default is 0.5.
+        threshold_weight : float, optional
+            The band centers with band weights lower than the threshhold weights 
+            are discarded. The default is None. If None, this is ignored.
+        mode : ['fatband','density', 'band_centers'], optional
+            Mode of plot. The default is "fatband".
+        yaxis_label : str, optional
+            Y-axis label text. The default is 'E (eV)'.
+        special_kpoints : dictionary, optional
+            Dictionary of special kpoints position and labels. If None, ignore
+            special kpoints. The default is None.
+        plotSC : bool, optional
+            Plot supercell bandstructure. The default is True.
+        marker : matplotlib.pyplot markerMarkerStyle, optional
+            The marker style. Marker can be either an instance of the class or 
+            the text shorthand for a particular marker. 
+            The default is 'o'.
+        fatfactor : int, optional
+            Scatter plot marker size. The default is 20.
+        nE : int, optional
+            Number of pixels in Energy scale when used 'density' mode. 
+            The default is 100.
+        smear : float, optional
+            Gaussian smearing. The default is 0.05.
+        color : str/color, optional
+            Color of plot of unfolded band structure. The color of supercell
+            band structures is gray. The default is 'gray'.
+        color_map: str/ matplotlib colormap
+            Colormap for density plot. The default is viridis.
+        show_legend : bool
+            If show legend or not. The default is True.
+        plot_colormap_bandcenter : bool, optional
+            If plotting the band ceneters by colormap. The default is True.
+
+        Returns
+        -------
+        fig : matplotlib.pyplot.figure
+            Figure instance. If ax is not None previously generated fig instance
+            will be used.
+        ax : Axis instance
+            Figure axis instance.
+        CountFig: int or None
+            Figure count.
+
+        """
+        
+        EBSplot.__init__(self, kpath_in_angs=kpath_in_angs, 
+                         unfolded_bandstructure=unfolded_bandstructure, 
+                         save_figure_dir=self.save_figure_directory)
+
+        return self.plot(ax=ax, save_file_name=save_file_name, CountFig=CountFig, Ef=Ef, 
+                         Emin=Emin, Emax=Emax, pad_energy_scale=pad_energy_scale, 
+                         threshold_weight=threshold_weight, mode=mode,
+                         yaxis_label=yaxis_label, special_kpoints=special_kpoints, 
+                         plotSC=plotSC, marker=marker, fatfactor=fatfactor, nE=nE, 
+                         smear=smear, color=color, color_map=color_map,
+                         plot_colormap_bandcenter=plot_colormap_bandcenter,
+                         show_legend=show_legend)
+        
+
```

### Comparing `banduppy-0.3.0/banduppy.egg-info/PKG-INFO` & `banduppy-0.3.1/banduppy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banduppy
-Version: 0.3.0
+Version: 0.3.1
 Summary: BandUPpy: Python interface of the BandUP code
 Home-page: https://www.ifm.liu.se/theomod/compphys/band-unfolding/
 Author: Stepan S. Tsirkin
 Author-email: stepan.tsirkin@ehu.eus
 Maintainer: Badal Mondal
 Maintainer-email: badalmondal.chembgc@gmail.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `banduppy-0.3.0/banduppy.egg-info/SOURCES.txt` & `banduppy-0.3.1/banduppy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `banduppy-0.3.0/setup.py` & `banduppy-0.3.1/setup.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-## python3 setup.py bdist_wheel
-## python3 -m twine upload dist/* 
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-     name='banduppy',  
-     author="Stepan S. Tsirkin",
-     author_email="stepan.tsirkin@ehu.eus",
-     maintainer="Badal Mondal",
-     maintainer_email="badalmondal.chembgc@gmail.com",
-     description="BandUPpy: Python interface of the BandUP code",
-     long_description=long_description,
-     long_description_content_type="text/markdown",
-     install_requires=['numpy', 'scipy >= 1.0', 'matplotlib' ,'irrep>=1.6.2'],
-     url="https://www.ifm.liu.se/theomod/compphys/band-unfolding/",
-     packages=setuptools.find_packages(),
-     classifiers=[
-         "Programming Language :: Python :: 3",
-         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-         "Operating System :: OS Independent",
-     ],
- )
+## python3 setup.py bdist_wheel
+## python3 -m twine upload dist/* 
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+     name='banduppy',  
+     author="Stepan S. Tsirkin",
+     author_email="stepan.tsirkin@ehu.eus",
+     maintainer="Badal Mondal",
+     maintainer_email="badalmondal.chembgc@gmail.com",
+     description="BandUPpy: Python interface of the BandUP code",
+     long_description=long_description,
+     long_description_content_type="text/markdown",
+     install_requires=['numpy', 'scipy >= 1.0', 'matplotlib' ,'irrep>=1.6.2'],
+     url="https://www.ifm.liu.se/theomod/compphys/band-unfolding/",
+     packages=setuptools.find_packages(),
+     classifiers=[
+         "Programming Language :: Python :: 3",
+         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+         "Operating System :: OS Independent",
+     ],
+ )
```

