# Comparing `tmp/daalab-1.0.tar.gz` & `tmp/daalab-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daalab-1.0.tar", last modified: Fri May 24 17:05:27 2024, max compression
+gzip compressed data, was "daalab-1.1.tar", last modified: Mon May 27 03:37:12 2024, max compression
```

## Comparing `daalab-1.0.tar` & `daalab-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-24 17:05:27.239251 daalab-1.0/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-24 17:05:27.239065 daalab-1.0/PKG-INFO
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      568 2024-05-23 10:49:22.000000 daalab-1.0/README.md
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-24 17:05:27.238228 daalab-1.0/daalab/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    32378 2024-05-24 17:01:11.000000 daalab-1.0/daalab/__init__.py
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    27786 2024-05-24 17:00:54.000000 daalab-1.0/daalab/codes.py
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)     1363 2024-05-24 02:29:40.000000 daalab-1.0/daalab/testing.py
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-24 17:05:27.238885 daalab-1.0/daalab.egg-info/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-24 17:05:27.000000 daalab-1.0/daalab.egg-info/PKG-INFO
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      191 2024-05-24 17:05:27.000000 daalab-1.0/daalab.egg-info/SOURCES.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        1 2024-05-24 17:05:27.000000 daalab-1.0/daalab.egg-info/dependency_links.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        7 2024-05-24 17:05:27.000000 daalab-1.0/daalab.egg-info/top_level.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       38 2024-05-24 17:05:27.239303 daalab-1.0/setup.cfg
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      269 2024-05-24 17:05:22.000000 daalab-1.0/setup.py
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-27 03:37:12.597422 daalab-1.1/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-27 03:37:12.597292 daalab-1.1/PKG-INFO
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      568 2024-05-23 10:49:22.000000 daalab-1.1/README.md
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-27 03:37:12.596366 daalab-1.1/daalab/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    31731 2024-05-27 03:01:50.000000 daalab-1.1/daalab/__init__.py
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    40506 2024-05-27 03:13:22.000000 daalab-1.1/daalab/codes.py
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)     1363 2024-05-24 02:29:40.000000 daalab-1.1/daalab/testing.py
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-27 03:37:12.597116 daalab-1.1/daalab.egg-info/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-27 03:37:12.000000 daalab-1.1/daalab.egg-info/PKG-INFO
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      191 2024-05-27 03:37:12.000000 daalab-1.1/daalab.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        1 2024-05-27 03:37:12.000000 daalab-1.1/daalab.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        7 2024-05-27 03:37:12.000000 daalab-1.1/daalab.egg-info/top_level.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       38 2024-05-27 03:37:12.597469 daalab-1.1/setup.cfg
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      269 2024-05-27 02:33:32.000000 daalab-1.1/setup.py
```

### Comparing `daalab-1.0/README.md` & `daalab-1.1/README.md`

 * *Files identical despite different names*

### Comparing `daalab-1.0/daalab/__init__.py` & `daalab-1.1/daalab/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .codes import print01, print_fk, print_huffman, print_queen1, print_queen2, print_graph_colour, print_matrixchain, print_tspbb, print_lcs, print_01bb, print_floyed, print_tspdp, print_jobseq, print_dijkstra, print_kruskal, print_prims, print_bellman, print_huffman2, print_graphcol2
+from .codes import print01, print_fk, print_huffman, print_queen1, print_queen2, print_graph_colour, print_matrixchain, print_tspbb, print_lcs, print_01bb, print_floyed, print_tspdp, print_jobseq, print_dijkstra, print_kruskal, print_prims, print_bellman, print_huffman2, print_graphcol2, print_react_form, print_react_timetable, print_react_func, print_react_sp, print_react_routes, print_react_es5_es6, print_form_validation, print_bootstrap_table
 
 zerone = print01
 fracknap = print_fk
 huffman = print_huffman
 queen1 = print_queen1
 queen2 = print_queen2
 graphcol = print_graph_colour
@@ -15,35 +15,31 @@
 jobseq = print_jobseq
 dijkstra = print_dijkstra
 kruskal = print_kruskal
 prims = print_prims
 bellman = print_bellman
 huffman2 = print_huffman2
 graphcol2 = print_graphcol2
+form = print_react_form
+table = print_react_timetable
+func_class = print_react_func
+states_props = print_react_sp
+routes = print_react_routes
+es5_es6 = print_react_es5_es6
+form_valid = print_form_validation
+bootstrap_table = print_bootstrap_table
 
 
 def list():
     functions = {
-    "zerone": "space complexity: O(nW) and time complexity: O(nW)",
-    "fracknap": "space complexity: O(n) and time complexity: O(n log n)",
-    "huffman": "space complexity: O(n) and time complexity: O(n log n)",
-    "queen1": "space complexity: O(n) and time complexity: O(n!)",
-    "queen2": "space complexity: O(n^2) and time complexity: O(n!)",
-    "graphcol": "space complexity: O(V) and time complexity: O(V+E)",
-    "matrixchain": "space complexity: O(n^2) and time complexity: O(n^3)",
-    "tspbb": "space complexity: O(n^2) and time complexity: O(n^2 * 2^n)",
-    "lcs": "space complexity: O(mn) and time complexity: O(mn)",
-    "zeronebb": "space complexity: O(n) and time complexity: O(2^n)",
-    "floyed": "space complexity: O(n^2) and time complexity: O(n^3)",
-    "tspdp": "space complexity: O(n * 2^n) and time complexity: O(n^2 * 2^n)",
-    "jobseq": "space complexity: O(n) and time complexity: O(n log n)",
-    "dijkstra": "space complexity: O(V^2) and time complexity: O(V^2)",
-    "kruskal": "space complexity: O(E) and time complexity: O(E log V)",
-    "prims": "space complexity: O(V+E) and time complexity: O(E logV)",
-    "bellman": "space complexity: O(V) and time complexity: O(VE)"
+#    form = print_react_form
+# table = print_react_timetable
+# func_class = print_react_func
+# states_props = print_react_sp
+# routes = print_react_routes
 }
 
 
     print("Available functions in the daalab library:")
     for name, description in functions.items():
         print(f"{name}: {description}")
```

### Comparing `daalab-1.0/daalab/codes.py` & `daalab-1.1/daalab/codes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1031,7 +1031,519 @@
     except ValueError as e:
         print(e)
 
 if __name__ == "__main__":
     main()'''
     print(code)
 
+
+
+def print_react_form():
+    code = '''import React, { useState } from 'react';
+
+const FormComponent = () => {
+  const [formData, setFormData] = useState({
+    name: '',
+    email: '',
+    password: ''
+  });
+
+  const handleChange = (event) => {
+    const { name, value } = event.target;
+    setFormData({
+      ...formData,
+      [name]: value
+    });
+  };
+
+  const handleSubmit = (event) => {
+    event.preventDefault();
+    alert(`Submitted Data:\nName: ${formData.name}\nEmail: ${formData.email}\nPassword: ${formData.password}`);
+  };
+
+  return (
+    <form onSubmit={handleSubmit}>
+      <div>
+        <label htmlFor="name">Name:</label>
+        <input
+          type="text"
+          id="name"
+          name="name"
+          value={formData.name}
+          onChange={handleChange}
+        />
+      </div>
+      <div>
+        <label htmlFor="email">Email:</label>
+        <input
+          type="email"
+          id="email"
+          name="email"
+          value={formData.email}
+          onChange={handleChange}
+        />
+      </div>
+      <div>
+        <label htmlFor="password">Password:</label>
+        <input
+          type="password"
+          id="password"
+          name="password"
+          value={formData.password}
+          onChange={handleChange}
+        />
+      </div>
+      <button type="submit">Submit</button>
+    </form>
+  );
+};
+
+export default FormComponent;
+'''
+    print(code)
+
+
+
+def print_react_timetable():
+    code = '''import React from 'react';
+
+const Timetable = () => {
+  return (
+    <div className="container mt-4">
+      <h3 className="text-center mb-4">CHAITANYA BHARATHI INSTITUTE OF TECHNOLOGY </h3>
+      <h3 className="text-center mb-4">DEPARTMENT OF COMPUTER ENGINEERING AND TECHNOLOGY</h3>
+      <h4 className="text-center mb-4">Class Time Table for the AY 2023-24    VI - Semester</h4>
+      <h4 className="text-center mb-4">Class B.E - VI Semester           W.E.F.: 12-02-2024           Room No. A-301</h4>
+      <table className="table table-bordered text-center">
+        <thead className="thead-dark">
+          <tr className='theaad'>
+            <th >
+            <div className="trow">
+                Period
+              </div>
+              <div className="trow">
+                Day/ Time
+              </div>
+            </th>
+            <th>
+            <div className="trow">
+                I
+              </div>
+              <div className="trow">
+              9:00 AM - 10:00 AM
+              </div>
+              </th>
+            <th>
+            <div className="trow">
+                II
+              </div>
+              <div className="trow">
+              10:10 AM - 11:10 AM
+              </div>
+              </th>
+            <th>
+            <div className="trow">
+                III
+              </div>
+              <div className="trow">
+              11:20 AM - 12:20 PM
+              </div></th>
+            <th className='luncho'>
+            12:20 PM - 1:10 PM</th>
+            <th>
+            <div className="trow">
+                IV
+              </div>
+              <div className="trow">
+              1:10 PM - 2:10 PM
+              </div></th>
+            <th>
+            <div className="trow">
+                V
+              </div>
+              <div className="trow">
+              2:20 PM - 3:20 PM
+              </div></th>
+            <th>
+            <div className="trow">
+                VI
+              </div>
+              <div className="trow">
+              3:30 PM - 4:30 PM
+              </div></th>
+          </tr>
+        </thead>
+        <tbody>
+          <tr>
+            <td className='greyed'>MONDAY</td>
+            <td>P.E II SC</td>
+            <td>SE</td>
+            <td>BPA</td>
+            <td className='lunch' rowSpan="6" style={{ writingMode: 'vertical-rl', textAlign: 'center', verticalAlign: 'middle' }}>LUNCH</td>
+            <td colSpan="3">BPA Lab @ TPO-1</td>
+            
+          </tr>
+          <tr>
+            <td className='greyed'>TUESDAY</td>
+            
+            <td>TOC</td>
+            <td colSpan="2">
+              <div className="trow">
+                UML Lab B2 @Lab -9
+              </div>
+              <div className="trow">
+                ES Lab B-1
+              </div>
+            </td>
+            <td>SE</td>
+            <td>PE-II SC @ A302, VAPT @A-301</td>
+            <td>UHV</td>
+          </tr>
+          <tr>
+            <td className='greyed'>WEDNESDAY</td>
+            <td>BPA</td>
+            <td>PE-II SCO Lab-9,VAPT@A-301</td>
+            <td>TOC</td>
+            <td>OE-II TWS@ A-301 FN @ Lab 9</td>
+            <td>UHV</td>
+            <td>SPORTS</td>
+          </tr>
+          <tr>
+            <td className='greyed'>THURSDAY</td>
+            <td>TOC</td>
+            <td>SE</td>
+            <td>LIBRARY</td>
+            <td>PE-II SC @ Lab-9, VAPT @A-301</td>
+            <td>BPA</td>
+            <td>OE TWS @ A-301, FM @A-302</td>
+          </tr>
+          <tr>
+            <td className='greyed'>FRIDAY</td>
+            <td>UHV</td>
+            <td>SE</td>
+            <td>OE TWS @ A-301, FM @A-302</td>
+            <td>MENTORING</td>
+            <td colSpan="2"><div className="trow">
+                UML Lab B1 @Lab -9
+              </div>
+              <div className="trow">
+                ES Lab B-2
+              </div></td>
+          </tr>
+          <tr>
+            <td className='greyed'>SATURDAY</td>
+            <td colSpan="2"><div className="trow">
+            PE-II:VAPT LAB ® TPO-3
+              </div>
+              <div className="trow">
+              PE-II:SC LAB ® Lab - 10
+              </div></td>
+            <td>BPA</td>
+            <td>TOC</td>
+            <td>OE-II TWS @ A-301</td>
+            <td></td>
+          </tr>
+        </tbody>
+      </table>
+    </div>
+  );
+};
+
+export default Timetable;
+'''
+    print(code)
+
+
+def print_react_sp():
+    code = '''import React from 'react';
+import ChildComponent from './ChildComponent';
+
+const ParentComponent = () => {
+  const parentData = "Data from Parent Component";
+
+  return (
+    <div>
+      <h1>Parent Component</h1>
+      <ChildComponent data={parentData} />
+    </div>
+  );
+};
+
+export default ParentComponent;
+
+
+
+import React, { useState } from 'react';
+
+const ChildComponent = ({ data }) => {
+  const [childData, setChildData] = useState("Initial Child Data");
+
+  const updateChildData = () => {
+    setChildData("Updated Child Data");
+  };
+
+  return (
+    <div>
+      <h2>Child Component</h2>
+      <p>{data}</p>
+      <p>{childData}</p>
+      <button onClick={updateChildData}>Update Child Data</button>
+    </div>
+  );
+};
+
+export default ChildComponent;
+'''
+    print(code)
+
+def print_react_func():
+    code = '''import React from 'react';
+
+const FunctionalComponent = () => {
+  return (
+    <div>
+      <h1>Hello, I am a Functional Component!</h1>
+    </div>
+  );
+};
+
+export default FunctionalComponent;
+
+
+
+import React, { Component } from 'react';
+
+class ClassComponent extends Component {
+  render() {
+    return (
+      <div>
+        <h1>Hello, I am a Class Component!</h1>
+      </div>
+    );
+  }
+}
+
+export default ClassComponent;
+'''
+    print(code)
+
+def print_react_routes():
+    code = '''
+//in this you will have to create the form.jsx and timetable.jsx or some other components 
+import React from 'react';
+import { BrowserRouter as Router, Route, Routes } from 'react-router-dom';
+import Timetable from './Timetable';
+import Form from './Form';
+import Home from './Home';
+import './App.css';
+
+function App() {
+  return (
+    <Router>
+      <div className="App">
+        <Routes>
+          <Route path="/timetable" element={<Timetable />} />
+          <Route path="/form" element={<Form />} />
+          <Route path="/" element={<Home/>} />
+        </Routes>
+      </div>
+    </Router>
+  );
+}
+
+export default App;
+
+
+//home.jsx:
+import React from 'react'
+import { useNavigate } from 'react-router-dom'
+
+const Home = () => {
+    const navigate = useNavigate();
+
+    const handleclicktimetable = (()=>{
+        navigate('/timetable')
+    })
+
+    const handleclickform = (()=>{
+        navigate('/form')
+    })
+
+  return (
+    <div className='home'>
+        <div className="button" onClick={handleclicktimetable}>
+            Open Timetable
+        </div>
+        <div className="button " onClick={handleclickform}>
+            Open Form
+        </div>
+    </div>
+  )
+}
+
+export default Home
+'''
+    print(code)
+
+
+def print_react_es5_es6():
+    code = '''// ES5 Version
+
+// Function to calculate factorial using traditional function declaration
+function factorialES5(num) {
+  if (num === 0 || num === 1) {
+    return 1;
+  } else {
+    return num * factorialES5(num - 1);
+  }
+}
+
+// Using the function to calculate factorial of 5
+console.log(factorialES5(5)); // Output: 120
+
+
+// ES6 Version
+
+// Function to calculate factorial using arrow function
+const factorialES6 = (num) => {
+  return (num === 0 || num === 1) ? 1 : num * factorialES6(num - 1);
+}
+
+// Using the function to calculate factorial of 5
+console.log(factorialES6(5)); // Output: 120'''
+    print(code)
+
+def print_form_validation():
+    code = '''<!DOCTYPE html>
+<html lang="en">
+<head>
+<meta charset="UTF-8">
+<title>Form Validation on Button Click</title>
+</head>
+<body>
+<form id="myForm" onsubmit="return validateForm()">
+    <label for="username">Username:</label>
+    <input type="text" id="username">
+    <br>
+
+    <label for="password">Password:</label>
+    <input type="password" id="password">
+    <br>
+
+    <label for="email">Email:</label>
+    <input type="email" id="email">
+    <br>
+
+    <button type="submit">Submit</button>
+</form>
+
+<script>
+function validateForm() {
+    event.preventDefault(); // Prevent form from submitting
+
+    var username = document.getElementById('username').value;
+    var password = document.getElementById('password').value;
+    var email = document.getElementById('email').value;
+
+    var usernameRegex = /^[a-zA-Z0-9]{3,16}$/;
+    var passwordRegex = /^(?=.*\d)(?=.*[a-z])(?=.*[A-Z])(?=.*\W).{8,}$/;
+    var emailRegex = /^[a-zA-Z0-9.%+_-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$/;
+
+    if (!usernameRegex.test(username)) {
+        alert('Enter a valid username.');
+        return false;
+    }
+
+    if (!passwordRegex.test(password)) {
+        alert('Enter a valid password.');
+        return false;
+    }
+
+    if (!emailRegex.test(email)) {
+        alert('Enter a valid email address.');
+        return false;
+    }
+
+    return true; // Only returns true if all validations pass
+}
+</script>
+</body>
+</html>
+'''
+    print(code)
+
+def print_bootstrap_table():
+    code = '''<!DOCTYPE html>
+<html lang="en">
+<head>
+    <meta charset="UTF-8">
+    <title>Enhanced Bootstrap Table</title>
+    <!-- Link to Bootstrap CSS for styling -->
+    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.min.css" rel="stylesheet">
+</head>
+<body>
+    <div class="container mt-3">
+        <h2>Feature-Rich Bootstrap Table</h2>
+        <!-- Table Responsive Wrapper -->
+        <div class="table-responsive">
+            <!-- Table with striped rows, hover effect, and bordered layout -->
+            <table class="table table-striped table-hover table-bordered">
+                <!-- Dark table header -->
+                <thead class="table-dark">
+                    <tr>
+                        <th>#</th>
+                        <th>First Name</th>
+                        <th>Last Name</th>
+                        <th>Email</th>
+                        <th>City</th>
+                    </tr>
+                </thead>
+                <tbody>
+                    <tr>
+                        <td>1</td>
+                        <td>John</td>
+                        <td>Doe</td>
+                        <td>john@example.com</td>
+                        <td>New York</td>
+                    </tr>
+                    <tr>
+                        <td>2</td>
+                        <td>Jane</td>
+                        <td>Doe</td>
+                        <td>jane@example.com</td>
+                        <td>Los Angeles</td>
+                    </tr>
+                    <tr>
+                        <td>3</td>
+                        <td>Jim</td>
+                        <td>Beam</td>
+                        <td>jim@example.com</td>
+                        <td>Chicago</td>
+                    </tr>
+                </tbody>
+            </table>
+        </div>
+    </div>
+</body>
+</html>
+'''
+    print(code)
+
+
+def print_crud():
+    code = '''
+mongo
+use myDatabase
+db.myCollection.insertOne({ name: "John", age: 30 })
+
+db.myCollection.findOne({ name: "John" })
+
+
+db.myCollection.updateOne({ name: "John" }, { $set: { age: 31 } })
+
+
+db.myCollection.findOne({ name: "John" })
+
+
+db.myCollection.deleteOne({ name: "John" })
+'''
+    print(code)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `daalab-1.0/daalab/testing.py` & `daalab-1.1/daalab/testing.py`

 * *Files identical despite different names*

