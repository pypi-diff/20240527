# Comparing `tmp/nqrduck_measurement-0.0.5.tar.gz` & `tmp/nqrduck_measurement-0.0.6.tar.gz`

## Comparing `nqrduck_measurement-0.0.5.tar` & `nqrduck_measurement-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0  5520293 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/docs/img/measurement_ui_labeled_v2.png
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/__init__.py
--rw-r--r--   0        0        0    10837 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/controller.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/measurement.py
--rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/model.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/signalprocessing_options.py
--rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/view.py
--rw-r--r--   0        0        0     9123 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/widget.py
--rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/resources/measurement_widget.ui
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/resources/mesurement.ini
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/LICENSE
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/README.md
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0  5520293 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/docs/img/measurement_ui_labeled_v2.png
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/src/nqrduck_measurement/__init__.py
+-rw-r--r--   0        0        0    11741 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/src/nqrduck_measurement/controller.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/src/nqrduck_measurement/measurement.py
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/src/nqrduck_measurement/model.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/src/nqrduck_measurement/signalprocessing_options.py
+-rw-r--r--   0        0        0    22485 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/src/nqrduck_measurement/view.py
+-rw-r--r--   0        0        0     9123 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/src/nqrduck_measurement/widget.py
+-rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/src/nqrduck_measurement/resources/measurement_widget.ui
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/src/nqrduck_measurement/resources/mesurement.ini
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/README.md
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.6/PKG-INFO
```

### Comparing `nqrduck_measurement-0.0.5/CHANGELOG.md` & `nqrduck_measurement-0.0.6/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## Version 0.0.6 (27-05-2024)
+
+- Added fitting functions to the measurement module (`dca1c6816f0697ca3c6827fd07a0236a3189b922`).
+
 ## Version 0.0.5 (20-05-2024)
 
 - Fixed measurement dialog not showing in wayland (`f5705e4efcbaf1aa0efd558b1ec1dacf42a53944`)
 - Measurement names are now editable (`be2e895c5768c3a82c329da62f9afef4bd953895`).
 - Improved darkmode compatibility (`be2e895c5768c3a82c329da62f9afef4bd953895`).
 
 ## Version 0.0.4 (05-05-2024)
```

### Comparing `nqrduck_measurement-0.0.5/.github/workflows/python-publish.yml` & `nqrduck_measurement-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.5/docs/img/measurement_ui_labeled_v2.png` & `nqrduck_measurement-0.0.6/docs/img/measurement_ui_labeled_v2.png`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.5/src/nqrduck_measurement/controller.py` & `nqrduck_measurement-0.0.6/src/nqrduck_measurement/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Controller for the measurement module."""
 
 import logging
 import json
 from PyQt6.QtCore import pyqtSlot, pyqtSignal
 from PyQt6.QtWidgets import QApplication
-from .signalprocessing_options import Apodization
+from .signalprocessing_options import Apodization, Fitting
 from nqrduck.module.module_controller import ModuleController
 from nqrduck_spectrometer.measurement import Measurement
 
 logger = logging.getLogger(__name__)
 
 
 class MeasurementController(ModuleController):
@@ -227,14 +227,44 @@
 
         apodized_measurement = measurement.apodization(function)
 
         dialog.deleteLater()
 
         self.module.model.displayed_measurement = apodized_measurement
         self.module.model.add_measurement(apodized_measurement)
+    
+    def show_fitting_dialog(self) -> None:
+        """Show fitting dialog."""
+        logger.debug("Showing fitting dialog.")
+        # First we  check if there is a measurement.
+        if not self.module.model.displayed_measurement:
+            logger.debug("No measurement to fit.")
+            self.module.nqrduck_signal.emit(
+                "notification", ["Error", "No measurement to fit."]
+            )
+            return
+
+        measurement = self.module.model.displayed_measurement
+
+        dialog = Fitting(measurement, parent=self.module.view)
+        result = dialog.exec()
+
+        logger.debug("Dialog result: %s", result)
+        if not result:
+            return
+
+        fit = dialog.get_fit()[1]
+
+        logger.debug("Fitting function: %s", fit)
+
+        measurement.add_fit(fit)
+
+        self.module.view.update_displayed_measurement()
+
+        dialog.deleteLater()
 
     @pyqtSlot()
     def change_displayed_measurement(self, measurement=None) -> None:
         """Change the displayed measurement.
 
         If no measurement is provided, the displayed measurement is changed to the selected measurement in the selection box.
```

### Comparing `nqrduck_measurement-0.0.5/src/nqrduck_measurement/model.py` & `nqrduck_measurement-0.0.6/src/nqrduck_measurement/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
         measurement_frequency_changed: Signal emitted when the measurement frequency changes.
         averages_changed: Signal emitted when the number of averages changes.
     """
 
     FILE_EXTENSION = "meas"
     # This constants are used to determine which view is currently displayed.
-    FFT_VIEW = "fft"
+    FFT_VIEW = "frequency"
     TIME_VIEW = "time"
 
     displayed_measurement_changed = pyqtSignal(Measurement)
     measurements_changed = pyqtSignal(list)
     
     view_mode_changed = pyqtSignal(str)
```

### Comparing `nqrduck_measurement-0.0.5/src/nqrduck_measurement/signalprocessing_options.py` & `nqrduck_measurement-0.0.6/src/nqrduck_measurement/signalprocessing_options.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """Signal processing options."""
 
 import logging
 import sympy
-from nqrduck_spectrometer.measurement import Measurement
+from nqrduck_spectrometer.measurement import Measurement, Fit, T2StarFit, LorentzianFit
 from nqrduck.helpers.functions import Function, GaussianFunction, CustomFunction
-from nqrduck.helpers.formbuilder import DuckFormBuilder, DuckFormFunctionSelectionField
+from nqrduck.helpers.formbuilder import (
+    DuckFormBuilder,
+    DuckFormFunctionSelectionField,
+    DuckFormDropdownField,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class FIDFunction(Function):
     """The exponetial FID function."""
 
@@ -19,15 +23,14 @@
         expr = sympy.sympify("exp( -x / T2star )")
         super().__init__(expr)
         self.start_x = 0
         self.end_x = 30
 
         self.add_parameter(Function.Parameter("T2star (microseconds)", "T2star", 10))
 
-
 class Apodization(DuckFormBuilder):
     """Apodization parameter.
 
     This parameter is used to apply apodization functions to the signal.
     The apodization functions are used to reduce the noise in the signal.
     """
 
@@ -47,18 +50,55 @@
         function_selection_field = DuckFormFunctionSelectionField(
             text=None,
             tooltip=None,
             functions=functions,
             duration=self.duration,
             parent=parent,
             default_function=0,
+            view_mode="time",
+            mode_selection=0,
         )
 
         self.add_field(function_selection_field)
 
     def get_function(self) -> Function:
         """Get the selected function.
 
         Returns:
             Function: The selected function.
         """
         return self.get_values()[0]
+
+
+class Fitting(DuckFormBuilder):
+    """Fitting parameter.
+
+    This parameter is used to apply fitting functions to the signal.
+    The fitting functions are used to reduce the noise in the signal.
+    """
+
+    def __init__(self, measurement: Measurement, parent=None) -> None:
+        """Fitting parameter."""
+        super().__init__("Fitting", parent=parent)
+
+        self.measurement = measurement
+
+        fits = {}
+        fits["T2*"] = T2StarFit(self.measurement)
+        fits["Lorentzian"] = LorentzianFit(self.measurement)
+
+        selection_field = DuckFormDropdownField(
+            text=None,
+            tooltip=None,
+            options=fits,
+            default_option=0,
+        )
+
+        self.add_field(selection_field)
+
+    def get_fit(self) -> Fit:
+        """Get the selected fit.
+
+        Returns:
+            Fit: The selected fit.
+        """
+        return self.get_values()[0]
```

### Comparing `nqrduck_measurement-0.0.5/src/nqrduck_measurement/view.py` & `nqrduck_measurement-0.0.6/src/nqrduck_measurement/view.py`

 * *Files 12% similar despite different names*

```diff
@@ -85,14 +85,18 @@
             self.on_set_averages_failure
         )
 
         self._ui_form.apodizationButton.clicked.connect(
             self.module.controller.show_apodization_dialog
         )
 
+        self._ui_form.fittingButton.clicked.connect(
+            self.module.controller.show_fitting_dialog
+        )
+
         # Add logos
         self._ui_form.buttonStart.setIcon(Logos.Play_16x16())
         self._ui_form.buttonStart.setIconSize(self._ui_form.buttonStart.size())
         self._ui_form.buttonStart.setEnabled(False)
 
         self._ui_form.exportButton.setIcon(Logos.Save16x16())
         self._ui_form.exportButton.setIconSize(self._ui_form.exportButton.size())
@@ -116,15 +120,15 @@
         # Set Min Max Values for frequency and averages
         self._ui_form.frequencyEdit.set_min_value(20.0)
         self._ui_form.frequencyEdit.set_max_value(1000.0)
 
         self._ui_form.averagesEdit.set_min_value(1)
         self._ui_form.averagesEdit.set_max_value(1e6)
 
-        # Connect selectionBox signal fors switching the displayed  measurement
+        # Connect selectionBox signal for switching the displayed  measurement
         self._ui_form.selectionBox.valueChanged.connect(
             self.module.controller.change_displayed_measurement
         )
 
     def init_plotter(self) -> None:
         """Initialize plotter with the according units for time domain."""
         plotter = self._ui_form.plotter
@@ -203,14 +207,17 @@
                 x, y.imag, label="Imaginary", linestyle="-", alpha=0.35, color="green"
             )
             # Magnitude
             self._ui_form.plotter.canvas.ax.plot(
                 x, np.abs(y), label="Magnitude", color="blue"
             )
 
+            # Plot fits
+            self.plot_fits()
+
             # Add legend
             self._ui_form.plotter.canvas.ax.legend()
 
             # Highlight the displayed measurement in the measurementsList
             for i in range(self._ui_form.measurementsList.count()):
                 item = self._ui_form.measurementsList.item(i)
                 widget = self._ui_form.measurementsList.itemWidget(item)
@@ -226,18 +233,58 @@
             for measurement in self.module.model.measurements:
                 if measurement.name == self.module.model.displayed_measurement.name:
                     self._ui_form.selectionBox.setValue(
                         self.module.model.measurements.index(measurement)
                     )
                     break
 
-        except AttributeError:
-            logger.debug("No measurement data to display.")
+        except AttributeError as e:
+            logger.debug(f"No measurement data to display: {e}")
+
         self._ui_form.plotter.canvas.draw()
 
+    def plot_fits(self):
+        """Plots the according fits to the displayed measurement if there are any and if the view mode is correct."""
+        measurement = self.module.model.displayed_measurement
+
+        if not measurement.fits:
+            logger.debug("No fits to plot.")
+            return
+
+        for fit in measurement.fits:
+            if fit.domain == self.module.model.view_mode:
+                logger.debug(f"Plotting {fit.name} fit in domain {fit.domain}.")
+                x = fit.x
+                y = fit.y
+                # Shift the x values if the view mode is FFT
+                if fit.domain == self.module.model.FFT_VIEW:
+                    x = x + float(
+                        measurement.target_frequency - measurement.IF_frequency
+                    ) * 1e-6
+
+                self._ui_form.plotter.canvas.ax.plot(
+                    x, y, label=f"{fit.name} Fit", linestyle="--"
+                )
+
+                # Add the parameters to the plot
+                offset = 0
+                for name, value in fit.parameters.items():
+                    if name == "covariance":
+                        continue
+
+                    # Only two digits after the comma
+                    value = round(value, 2)
+
+                    self._ui_form.plotter.canvas.ax.text(
+                        max(x) / 90,
+                        max(y) / 2 + offset,
+                        f"{name}: {value}",
+                    )
+                    offset += max(y) / 10
+
     @pyqtSlot()
     def on_measurement_start_button_clicked(self) -> None:
         """Slot for when the measurement start button is clicked."""
         logger.debug("Measurement start button clicked.")
         self.module.controller.start_measurement()
 
     @pyqtSlot()
@@ -254,27 +301,27 @@
 
     @pyqtSlot()
     def on_measurement_save_button_clicked(self) -> None:
         """Slot for when the measurement save button is clicked."""
         logger.debug("Measurement save button clicked.")
 
         file_manager = self.FileManager(
-            self.module.model.FILE_EXTENSION, parent=self.widget
+            self.module.model.FILE_EXTENSION, parent=self
         )
         file_name = file_manager.saveFileDialog()
         if file_name:
             self.module.controller.save_measurement(file_name)
 
     @pyqtSlot()
     def on_measurement_load_button_clicked(self) -> None:
         """Slot for when the measurement load button is clicked."""
         logger.debug("Measurement load button clicked.")
 
         file_manager = self.FileManager(
-            self.module.model.FILE_EXTENSION, parent=self.widget
+            self.module.model.FILE_EXTENSION, parent=self
         )
         file_name = file_manager.loadFileDialog()
         if file_name:
             self.module.controller.load_measurement(file_name)
 
     @pyqtSlot()
     def on_measurements_changed(self) -> None:
@@ -383,26 +430,28 @@
             """Initialize the dialog."""
             super().__init__(parent)
             self.setParent(parent)
             self.finished = False
             self.setModal(True)
             self.setWindowFlag(Qt.WindowType.FramelessWindowHint)
             self.setAttribute(Qt.WidgetAttribute.WA_TranslucentBackground)
-            self.setWindowFlag(Qt.WindowType.WindowStaysOnTopHint)  # Ensure the window stays on top
+            self.setWindowFlag(
+                Qt.WindowType.WindowStaysOnTopHint
+            )  # Ensure the window stays on top
 
             self.message_label = QLabel("Measuring...")
             # Make label bold and text larger
             font = self.message_label.font()
             font.setPointSize(20)
             font.setBold(True)
             self.message_label.setFont(font)
 
             self.spinner_movie = DuckAnimations.DuckKick128x128()
             self.spinner_label = QLabel(self)
-            # Make spinner label 
+            # Make spinner label
             self.spinner_label.setMovie(self.spinner_movie)
 
             self.layout = QVBoxLayout(self)
             self.layout.addWidget(self.message_label)
             self.layout.addWidget(self.spinner_label)
 
             self.spinner_movie.finished.connect(self.on_movie_finished)
@@ -421,61 +470,124 @@
         def hide(self) -> None:
             """Hide the dialog and stop the spinner movie."""
             self.spinner_movie.stop()
             super().hide()
 
     class MeasurementEdit(QDialog):
         """This dialog is displayed when the measurement edit button is clicked.
-
-        It allows the user to edit the measurement parameters (e.g. name, ...)
+        
+        It allows the user to edit the measurement parameters (e.g. name, ...).
         """
 
         def __init__(self, measurement, parent=None) -> None:
             """Initialize the dialog."""
             super().__init__(parent)
             self.setParent(parent)
 
             self.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding)
-
             logger.debug("Edit measurement dialog started.")
 
             self.measurement = measurement
-
             self.setWindowTitle("Edit Measurement")
+
             self.layout = QVBoxLayout(self)
             self.setLayout(self.layout)
 
+            self.setup_name_section()
+            self.setup_fit_section()
+            self.setup_buttons()
+
+            # Resize the dialog
+            self.adjustSize()
+
+        def setup_name_section(self):
+            """Sets up the name layout section."""
             self.name_layout = QHBoxLayout()
             self.name_label = QLabel("Name:")
-            self.name_edit = QLineEdit(measurement.name)
+
+            self.name_edit = QLineEdit(self.measurement.name)
             font_metrics = self.name_edit.fontMetrics()
-            self.name_edit.setFixedWidth(
-                font_metrics.horizontalAdvance(self.name_edit.text()) + 10
-            )
+            self.name_edit.setFixedWidth(font_metrics.horizontalAdvance(
+                self.name_edit.text()) + 10)
             self.name_edit.adjustSize()
 
             self.name_layout.addWidget(self.name_label)
             self.name_layout.addWidget(self.name_edit)
+            self.layout.addLayout(self.name_layout)
 
+        def setup_fit_section(self):
+            """Sets up the fit layout section."""
+            self.fit_layout = QVBoxLayout()
+            self.update_fit_info()
+            self.layout.addLayout(self.fit_layout)
+
+        def setup_buttons(self):
+            """Sets up the OK and Cancel buttons."""
             self.ok_button = QPushButton("OK")
             self.ok_button.clicked.connect(self.on_ok_button_clicked)
 
             self.cancel_button = QPushButton("Cancel")
             self.cancel_button.clicked.connect(self.close)
 
-            self.layout.addLayout(self.name_layout)
-
             button_layout = QHBoxLayout()
             button_layout.addWidget(self.cancel_button)
             button_layout.addWidget(self.ok_button)
-
             self.layout.addLayout(button_layout)
 
-            # Resize the dialog
-            self.adjustSize()
+        def update_fit_info(self) -> None:
+            """Adds the associated fits to the dialog."""
+            # Clear the layout from previous fits
+            while self.fit_layout.count():
+                item = self.fit_layout.takeAt(0)
+                if item.widget():
+                    item.widget().deleteLater()
+                elif item.layout():
+                    self.clearLayout(item.layout())
+
+            if not self.measurement.fits:
+                logger.debug("No fits to display.")
+                return
+
+            # Adds the fit information
+            fit_label = QLabel("Fits:")
+            self.fit_layout.addWidget(fit_label)
+
+            for fit in self.measurement.fits:
+                specific_fit_layout = QHBoxLayout()
+                specific_fit_layout.addStretch()
+                logger.debug(f"Fit: {fit.name}")
+
+                fit_name_edit = QLineEdit(fit.name)
+                fit_name_edit.textChanged.connect(
+                    lambda text, fit=fit: self.measurement.edit_fit_name(fit, text)
+                )
+
+                fit_delete_button = QPushButton()
+                fit_delete_button.setIcon(Logos.Garbage12x12())
+                fit_delete_button.clicked.connect(partial(self.on_delete_fit, fit))
+
+                specific_fit_layout.addWidget(fit_name_edit)
+                specific_fit_layout.addWidget(fit_delete_button)
+                self.fit_layout.addLayout(specific_fit_layout)
+
+        def clearLayout(self, layout):
+            """Clears all items in the given layout."""
+            while layout.count():
+                item = layout.takeAt(0)
+                if item.widget():
+                    item.widget().deleteLater()
+                elif item.layout():
+                    self.clearLayout(item.layout())
+
+        def on_delete_fit(self, fit) -> None:
+            """Slot for when the delete fit button is clicked."""
+            logger.debug(f"Delete fit {fit.name}.")
+            self.measurement.delete_fit(fit)
+            self.update_fit_info()  # Update the dialog with the changes
 
         def on_ok_button_clicked(self) -> None:
             """Slot for when the OK button is clicked."""
             logger.debug("OK button clicked.")
             self.measurement.name = self.name_edit.text()
             self.accept()
             self.close()
+
```

### Comparing `nqrduck_measurement-0.0.5/src/nqrduck_measurement/widget.py` & `nqrduck_measurement-0.0.6/src/nqrduck_measurement/widget.py`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.5/src/nqrduck_measurement/resources/measurement_widget.ui` & `nqrduck_measurement-0.0.6/src/nqrduck_measurement/resources/measurement_widget.ui`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.5/LICENSE` & `nqrduck_measurement-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.5/README.md` & `nqrduck_measurement-0.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 # NQRduck Module: nqrduck-measurement
 
 A module for the [nqrduck](https://github.com/nqrduck/nqrduck) project. This module is used for single frequency magnetic resonance experiments.
 
 ## Installation
 
 ### Requirements
+
 Dependencies are handled via the pyproject.toml file.
 
 ### Setup
+
 To install the module you need the NQRduck core. You can find the installation instructions for the NQRduck core [here](https://github.com/nqrduck/nqrduck).
 
 Ideally you should install the module in a virtual environment. You can create a virtual environment by running the following command in the terminal:
+
 ```bash
 python -m venv nqrduck
 # Activate the virtual environment
 . nqrduck/bin/activate
 ```
 
 You can install this module and the dependencies by running the following command in the terminal while the virtual environment is activated and you are in the root directory of this module:
+
 ```bash
 pip install .
 ```
 
 Alternatively, you can install the module and the dependencies by running the following command in the terminal while the virtual environment is activated:
+
 ```bash
 pip install nqrduck-measurement
 ```
 
 ## Usage
+
 The module is used with the [Spectrometer](https://github.com/nqrduck/nqrduck-spectrometer) module. However you need to use an actual submodule of the spectrometer module like:
 
 - [nqrduck-spectrometer-limenqr](https://github.com/nqrduck/nqrduck-spectrometer-limenqr) A module used for magnetic resonance experiments with the LimeSDR (USB or Mini 2.0).
 - [nqrduck-spectrometer-simulator](https://github.com/nqrduck/nqrduck-spectrometer-simulator) A module used for simulating magnetic resonance experiments.
 
-The pulse sequence and spectrometer settings can be adjusted using the 'Spectrometer' tab. 
+The pulse sequence and spectrometer settings can be adjusted using the 'Spectrometer' tab.
 
 <img src="https://github.com/nqrduck/nqrduck-measurement/raw/0b28ae6b33230c6ca9eda85bd18de7cbcade27d1/docs/img/measurement_ui_labeled_v2.png" alt="drawing" width="800">
 
 - a.) The experiments settings for frequency and number of averages.
 - b.) The signal processing settings for the measurement.
 - c.) The 'Measurement Plot'. Here the measured data is displayed. One can switch time and frequency domain plots.
 - d.) The import and export buttons for the measurement data.
 
+You can then remove the folder of the virtual environment.
+
 ## License
+
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
 
 ## Contributing
+
 If you're interested in contributing to the project, start by checking out our [nqrduck-module template](https://github.com/nqrduck/nqrduck-module). To contribute to existing modules, please first open an issue in the respective module repository to discuss your ideas or report bugs.
```

### Comparing `nqrduck_measurement-0.0.5/pyproject.toml` & `nqrduck_measurement-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "nqrduck-measurement"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "A module for the NQRduck program (a simple python script™) to perform single frequency measurements."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `nqrduck_measurement-0.0.5/PKG-INFO` & `nqrduck_measurement-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nqrduck-measurement
-Version: 0.0.5
+Version: 0.0.6
 Summary: A module for the NQRduck program (a simple python script™) to perform single frequency measurements.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck-measurement/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck-measurement
 Author-email: jupfi <support@nqrduck.cool>
 License: MIT License
         
@@ -48,49 +48,59 @@
 # NQRduck Module: nqrduck-measurement
 
 A module for the [nqrduck](https://github.com/nqrduck/nqrduck) project. This module is used for single frequency magnetic resonance experiments.
 
 ## Installation
 
 ### Requirements
+
 Dependencies are handled via the pyproject.toml file.
 
 ### Setup
+
 To install the module you need the NQRduck core. You can find the installation instructions for the NQRduck core [here](https://github.com/nqrduck/nqrduck).
 
 Ideally you should install the module in a virtual environment. You can create a virtual environment by running the following command in the terminal:
+
 ```bash
 python -m venv nqrduck
 # Activate the virtual environment
 . nqrduck/bin/activate
 ```
 
 You can install this module and the dependencies by running the following command in the terminal while the virtual environment is activated and you are in the root directory of this module:
+
 ```bash
 pip install .
 ```
 
 Alternatively, you can install the module and the dependencies by running the following command in the terminal while the virtual environment is activated:
+
 ```bash
 pip install nqrduck-measurement
 ```
 
 ## Usage
+
 The module is used with the [Spectrometer](https://github.com/nqrduck/nqrduck-spectrometer) module. However you need to use an actual submodule of the spectrometer module like:
 
 - [nqrduck-spectrometer-limenqr](https://github.com/nqrduck/nqrduck-spectrometer-limenqr) A module used for magnetic resonance experiments with the LimeSDR (USB or Mini 2.0).
 - [nqrduck-spectrometer-simulator](https://github.com/nqrduck/nqrduck-spectrometer-simulator) A module used for simulating magnetic resonance experiments.
 
-The pulse sequence and spectrometer settings can be adjusted using the 'Spectrometer' tab. 
+The pulse sequence and spectrometer settings can be adjusted using the 'Spectrometer' tab.
 
 <img src="https://github.com/nqrduck/nqrduck-measurement/raw/0b28ae6b33230c6ca9eda85bd18de7cbcade27d1/docs/img/measurement_ui_labeled_v2.png" alt="drawing" width="800">
 
 - a.) The experiments settings for frequency and number of averages.
 - b.) The signal processing settings for the measurement.
 - c.) The 'Measurement Plot'. Here the measured data is displayed. One can switch time and frequency domain plots.
 - d.) The import and export buttons for the measurement data.
 
+You can then remove the folder of the virtual environment.
+
 ## License
+
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
 
 ## Contributing
+
 If you're interested in contributing to the project, start by checking out our [nqrduck-module template](https://github.com/nqrduck/nqrduck-module). To contribute to existing modules, please first open an issue in the respective module repository to discuss your ideas or report bugs.
```

