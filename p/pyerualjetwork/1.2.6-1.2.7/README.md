# Comparing `tmp/pyerualjetwork-1.2.6.tar.gz` & `tmp/pyerualjetwork-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.2.6.tar", last modified: Sun May 26 16:55:01 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.2.7.tar", last modified: Mon May 27 17:42:07 2024, max compression
```

## Comparing `pyerualjetwork-1.2.6.tar` & `pyerualjetwork-1.2.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 16:55:01.852548 pyerualjetwork-1.2.6/
--rw-rw-rw-   0        0        0      480 2024-05-26 16:55:01.851556 pyerualjetwork-1.2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-26 16:55:01.838412 pyerualjetwork-1.2.6/plan/
--rw-rw-rw-   0        0        0      352 2024-05-26 16:54:28.000000 pyerualjetwork-1.2.6/plan/__init__.py
--rw-rw-rw-   0        0        0    40107 2024-05-26 16:53:09.000000 pyerualjetwork-1.2.6/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:55:01.848561 pyerualjetwork-1.2.6/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      480 2024-05-26 16:55:01.000000 pyerualjetwork-1.2.6/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-26 16:55:01.000000 pyerualjetwork-1.2.6/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 16:55:01.000000 pyerualjetwork-1.2.6/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-26 16:55:01.000000 pyerualjetwork-1.2.6/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 16:55:01.853546 pyerualjetwork-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      656 2024-05-26 16:53:41.000000 pyerualjetwork-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 17:42:07.534721 pyerualjetwork-1.2.7/
+-rw-rw-rw-   0        0        0      446 2024-05-27 17:42:07.533649 pyerualjetwork-1.2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 17:42:07.500760 pyerualjetwork-1.2.7/plan/
+-rw-rw-rw-   0        0        0      352 2024-05-26 16:54:30.000000 pyerualjetwork-1.2.7/plan/__init__.py
+-rw-rw-rw-   0        0        0    40428 2024-05-27 17:26:14.000000 pyerualjetwork-1.2.7/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-27 17:42:07.531569 pyerualjetwork-1.2.7/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      446 2024-05-27 17:42:06.000000 pyerualjetwork-1.2.7/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-27 17:42:07.000000 pyerualjetwork-1.2.7/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 17:42:06.000000 pyerualjetwork-1.2.7/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-27 17:42:06.000000 pyerualjetwork-1.2.7/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 17:42:07.535724 pyerualjetwork-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      622 2024-05-27 17:37:32.000000 pyerualjetwork-1.2.7/setup.py
```

### Comparing `pyerualjetwork-1.2.6/plan/plan.py` & `pyerualjetwork-1.2.7/plan/plan.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,81 +8,81 @@
 # BUILD -----
 def TrainPLAN(
     TrainInputs: List[Union[int, float]], 
     TrainLabels: List[Union[int, float, str]], # At least two.. and one hot encoded
     ClassCount: int,
     Layers: List[str],
     Neurons: List[Union[int, float]],
-    ThresholdSigns: List[str],
-    ThresholdValues: List[Union[int, float]],
+    MembranThresholds: List[str],
+    MembranPotentials: List[Union[int, float]],
     Normalizations: List[str],
     Activations: List[str]
 ) -> str:
         
     infoPLAN = """
     Creates and configures a PLAN model.
     
     Args:
         TrainInputs (list[num]): List of input data.
         TrainLabels (list[num]): List of TrainLabels. (one hot encoded)
         ClassCount (int): Number of classes.
         Layers (list[str]): List of layer names. (options: 'fex' (Feature Extraction), 'cat' (Catalyser))
         Neurons (list[num]): List of neuron counts for each layer.
-        ThresholdSigns (list[str]): List of threshold signs.
-        ThresholdValues (list[num]): List of threshold values.
+        MembranThresholds (list[str]): List of MembranThresholds.
+        MembranPotentials (list[num]): List of MembranPotentials.
         Normalizations (List[str]): Whether normalization will be performed at indexed layers ("y" or "n").
         Activations (list[str]): List of activation functions.
     
     Returns:
         list([num]): (Weight matrices list, TrainPredictions list, TrainAcc).
         error handled ?: Process status ('e')
 """
         
     LastNeuron = Neurons[-1:][0]
     if LastNeuron != ClassCount:
             print(Fore.RED + "ERROR108: Last layer of neuron count must be equal class count. from: TrainPLAN",infoPLAN)
             return 'e'
     
-    if len(Normalizations) != len(ThresholdValues):
+    if len(Normalizations) != len(MembranPotentials):
         
-            print(Fore.RED + "ERROR307: Normalization list length must be equal to length of ThresholdSigns List,ThresholdValues List,Layers List,Neurons List. from: TrainPLAN",infoPLAN)
+            print(Fore.RED + "ERROR307: Normalization list length must be equal to length of MembranThresholds List,MembranPotentials List,Layers List,Neurons List. from: TrainPLAN",infoPLAN)
             return 'e'
     
     if len(TrainInputs) != len(TrainLabels):
         print(Fore.RED + "ERROR301: TrainInputs list and TrainLabels list must be same length.",infoPLAN)
         return 'e'
     
-    for i, Value in enumerate(ThresholdValues):
+    for i, Value in enumerate(MembranPotentials):
         
         if Normalizations[i] != 'y' and Normalizations[i] != 'n':
                 print(Fore.RED + "ERROR105: Normalization list must be 'y' or 'n'.",infoPLAN)
                 return 'e'
             
-        if ThresholdSigns[i] == 'none':
+        if MembranThresholds[i] == 'none':
             print(Fore.MAGENTA + "WARNING102: We are advise to do not put 'none' Threshold sign. But some cases improves performance of the model from: TrainPLAN",infoPLAN  + Style.RESET_ALL)
             time.sleep(3)
             
         if isinstance(Value, str):
-            print(Fore.RED + "ERROR201: Threshold values must be numeric. from: TrainPLAN")
+            print(Fore.RED + "ERROR201: MEMBRAN POTENTIALS must be numeric. from: TrainPLAN")
             return 'e'
         
         if isinstance(Neurons[i], str):
             print(Fore.RED + "ERROR202: Neurons list must be numeric.")
             return 'e'
     
-    if len(ThresholdSigns) != len(ThresholdValues):
-        print(Fore.RED + "ERROR302: Threshold signs list and Threshold Values list must be same length. from: TrainPLAN",infoPLAN)
+    if len(MembranThresholds) != len(MembranPotentials):
+        print(Fore.RED + "ERROR302: MEMBRAN THRESHOLDS list and MEMBRAN POTENTIALS list must be same length. from: TrainPLAN",infoPLAN)
         return 'e'
     
     if len(Layers) != len(Neurons):
         print(Fore.RED + "ERROR303: Layers list and Neurons list must same length. from: TrainPLAN",infoPLAN)
         return 'e'
     
-    if len(ThresholdValues) != len(Layers) or len(ThresholdSigns) != len(Layers):
-        print(Fore.RED + "ERROR306: Threshold Values and Threshold Signs lists length must be same Layers list length. from: TrainPLAN",infoPLAN)
+    if len(MembranPotentials) != len(Layers) or len(MembranThresholds) != len(Layers):
+        print(Fore.RED + "ERROR306: MEMBRAN POTENTIALS and MEMBRAN THRESHOLDS lists length must be same Layers list length. from: TrainPLAN",infoPLAN)
         return 'e'
     
     
     for Activation in Activations:
         if Activation != 'softmax' and Activation != 'sigmoid' and Activation != 'relu' and Activation != 'none':
             print(Fore.RED + "ERROR108: Activations list must be 'sigmoid' or 'softmax' or 'relu' or 'none' from: TrainPLAN",infoPLAN)
             return 'e'
@@ -101,22 +101,22 @@
             print(Fore.RED + "ERROR102: Neuron count must be greater than class count(For PLAN). from: TrainPLAN")
             return 'e'
         
         if Layers[index] != 'fex' and Layers[index] != 'cat':
             print(Fore.RED + "ERROR107: Layers list must be 'fex'(Feature Extraction Layer) or 'cat' (Catalyser Layer). from: TrainPLAN",infoPLAN)
             return 'e'
     
-    if len(ThresholdSigns) != len(ThresholdValues):
-        print(Fore.RED + "ERROR305: Threshold signs list and Threshold values list must be same length. from: TrainPLAN",infoPLAN)
+    if len(MembranThresholds) != len(MembranPotentials):
+        print(Fore.RED + "ERROR305: MEMBRAN THRESHOLDS list and MEMBRAN POTENTIALS list must be same length. from: TrainPLAN",infoPLAN)
         return 'e'
     
     
-    for i, Sign in enumerate(ThresholdSigns):
+    for i, Sign in enumerate(MembranThresholds):
         if Sign != '>' and Sign != '<' and Sign != '==' and Sign != '!=' and Sign != 'none':
-            print(Fore.RED + "ERROR104: Threshold signs must be '>' or '<' or '==' or '!='. or 'none' from: TrainPLAN",infoPLAN)
+            print(Fore.RED + "ERROR104: MEMBRAN THRESHOLDS must be '>' or '<' or '==' or '!='. or 'none' WE SUGGEST '<' FOR FEX LAYER AND '==' FOR CAT LAYER (Your data, your hyperparameter) from: TrainPLAN",infoPLAN)
             return 'e'
         
         if Layers[i] == 'fex' and Sign == 'none':
             print(Fore.RED + "ERROR109: at layer type 'fex', pairing with 'none' Threshold is not acceptlable. if you want to 'none' put '==' and make threshold value '0'. from: TrainPLAN ",infoPLAN)
             return 'e'
         
     UniqueTrainLabels = set()
@@ -177,17 +177,17 @@
                 NeuralLayer = Relu(NeuralLayer)
             elif Activations[Lindex] == 'sigmoid':
                 NeuralLayer = Sigmoid(NeuralLayer)
             elif Activations[Lindex] == 'softmax':
                 NeuralLayer = Softmax(NeuralLayer)
                 
             if Layer == 'fex':
-                NeuralLayer,W[Lindex] = Fex(NeuralLayer, W[Lindex], ThresholdSigns[Lindex], ThresholdValues[Lindex])
+                NeuralLayer,W[Lindex] = Fex(NeuralLayer, W[Lindex], MembranThresholds[Lindex], MembranPotentials[Lindex])
             elif Layer == 'cat':
-                NeuralLayer,W[Lindex] = Cat(NeuralLayer, W[Lindex], ThresholdSigns[Lindex], ThresholdValues[Lindex],1)
+                NeuralLayer,W[Lindex] = Cat(NeuralLayer, W[Lindex], MembranThresholds[Lindex], MembranPotentials[Lindex],1)
                 
         RealOutput = np.argmax(TrainLabels[index])
         PredictedOutput = np.argmax(NeuralLayer)
         if RealOutput == PredictedOutput:
             true += 1
         Acc = true / len(TrainLabels)
         TrainPredictions[index] = PredictedOutput
@@ -387,74 +387,74 @@
         
     return Divides
         
 
 def Fex(
     Input,               # list[num]: Input data.
     w,                   # list[list[num]]: Weight matrix of the neural network.
-    ThresholdsSign,      # str: Sign for threshold comparison ('<', '>', '==', '!=').
-    ThresholdValue       # num: Threshold value for comparison.
+    MembranThreshold,      # str: Sign for threshold comparison ('<', '>', '==', '!=').
+    MembranPotential       # num: Threshold value for comparison.
 ) -> tuple:
     """
     Applies feature extraction process to the input data using synaptic pruning.
 
     Args:
         Input (list[num]): Input data.
         w (list[list[num]]): Weight matrix of the neural network.
-        ThresholdsSign (str): Sign for threshold comparison ('<', '>', '==', '!=').
-        ThresholdValue (num): Threshold value for comparison.
+        MembranThreshold (str): Sign for threshold comparison ('<', '>', '==', '!=').
+        MembranPotential (num): Threshold value for comparison.
 
     Returns:
         tuple: A tuple (vector) containing the neural layer result and the updated weight matrix.
     """
 
-    if ThresholdsSign == '<':
-        PruneIndex = np.where(Input < ThresholdValue)
-    elif ThresholdsSign == '>': 
-        PruneIndex = np.where(Input > ThresholdValue)
-    elif ThresholdsSign == '==':
-        PruneIndex = np.where(Input == ThresholdValue)
-    elif ThresholdsSign == '!=':
-        PruneIndex = np.where(Input != ThresholdValue)
+    if MembranThreshold == '<':
+        PruneIndex = np.where(Input < MembranPotential)
+    elif MembranThreshold == '>': 
+        PruneIndex = np.where(Input > MembranPotential)
+    elif MembranThreshold == '==':
+        PruneIndex = np.where(Input == MembranPotential)
+    elif MembranThreshold == '!=':
+        PruneIndex = np.where(Input != MembranPotential)
 
     w = SynapticPruning(w, PruneIndex, 'col', 0, 0)
 
     NeuralLayer = np.dot(w, Input)
     return NeuralLayer,w
 
 def Cat(
     Input,               # list[num]: Input data.
     w,                   # list[list[num]]: Weight matrix of the neural network.
-    ThresholdsSign,      # str: Sign for threshold comparison ('<', '>', '==', '!=').
-    ThresholdValue,      # num: Threshold value for comparison.
+    MembranThreshold,      # str: Sign for threshold comparison ('<', '>', '==', '!=').
+    MembranPotential,      # num: Threshold value for comparison.
     isTrain              # int: Flag indicating if the function is called during training (1 for training, 0 otherwise).
 ) -> tuple:
     """
     Applies categorization process to the input data using synaptic pruning if specified.
 
     Args:
         Input (list[num]): Input data.
         w (list[list[num]]): Weight matrix of the neural network.
-        ThresholdsSign (str): Sign for threshold comparison ('<', '>', '==', '!=').
-        ThresholdValue (num): Threshold value for comparison.
+        MembranThreshold (str): Sign for threshold comparison ('<', '>', '==', '!=').
+        MembranPotential (num): Threshold value for comparison.
         isTrain (int): Flag indicating if the function is called during training (1 for training, 0 otherwise).
 
     Returns:
         tuple: A tuple containing the neural layer (vector) result and the possibly updated weight matrix.
     """
 
-    if ThresholdsSign == '<':     
-        PruneIndex = np.where(Input < ThresholdValue)
-    elif ThresholdsSign == '>':     
-        PruneIndex = np.where(Input > ThresholdValue)
-    elif ThresholdsSign == '==':
-        PruneIndex = np.where(Input == ThresholdValue)
-    elif ThresholdsSign == '!=':     
-        PruneIndex = np.where(Input != ThresholdValue)
-    if isTrain == 1 and ThresholdsSign != 'none':
+    if MembranThreshold == '<':     
+        PruneIndex = np.where(Input < MembranPotential)
+    elif MembranThreshold == '>':     
+        PruneIndex = np.where(Input > MembranPotential)
+    elif MembranThreshold == '==':
+        PruneIndex = np.where(Input == MembranPotential)
+    elif MembranThreshold == '!=':     
+        PruneIndex = np.where(Input != MembranPotential)
+    if isTrain == 1 and MembranThreshold != 'none':
      
             w = SynapticPruning(w, PruneIndex, 'col', 0, 0)
      
     
     NeuralLayer = np.dot(w, Input)
     return NeuralLayer,w
 
@@ -530,29 +530,29 @@
     return np.maximum(0, x)
 
 
 def TestPLAN(
     TestInputs,         # list[list[num]]: Test input data.
     TestLabels,         # list[num]: Test labels.
     Layers,             # list[str]: List of layer names.
-    ThresholdSigns,     # list[str]: List of threshold signs for each layer.
-    ThresholdValues,    # list[num]: List of threshold values for each layer.
+    MembranThresholds,     # list[str]: List of MEMBRAN THRESHOLDS for each layer.
+    MembranPotentials,    # list[num]: List of MEMBRAN POTENTIALS for each layer.
     Normalizations,    # str: Whether normalization will be performed ("y" or "n").
     Activations,         # str: Activation function list for the neural network.
     W                  # list[list[num]]: Weight matrix of the neural network.
 ) -> tuple:
     infoTestModel =  """
     Tests the neural network model with the given test data.
 
     Args:
         TestInputs (list[list[num]]): Test input data.
         TestLabels (list[num]): Test labels.
         Layers (list[str]): List of layer names.
-        ThresholdSigns (list[str]): List of threshold signs for each layer.
-        ThresholdValues (list[num]): List of threshold values for each layer.
+        MembranThresholds (list[str]): List of MEMBRAN THRESHOLDS for each layer.
+        MembranPotentials (list[num]): List of MEMBRAN POTENTIALS for each layer.
         Normalizatios list([str]): Whether normalization will be performed ("yes" or "no").
         Activation (str): Activation function for the neural network.
         W (list[list[num]]): Weight matrix of the neural network.
 
     Returns:
         tuple: A tuple containing the predicted labels and the accuracy of the model.
     """
@@ -581,17 +581,17 @@
                         NeuralLayer = Relu(NeuralLayer)
                 elif Activations[index] == 'sigmoid':
                         NeuralLayer = Sigmoid(NeuralLayer)
                 elif Activations[index] == 'softmax':
                         NeuralLayer = Softmax(NeuralLayer)
                         
                 if Layers[index] == 'fex':
-                    NeuralLayer,useless = Fex(NeuralLayer, W[index], ThresholdSigns[index], ThresholdValues[index])
+                    NeuralLayer,useless = Fex(NeuralLayer, W[index], MembranThresholds[index], MembranPotentials[index])
                 if Layers[index] == 'cat':
-                    NeuralLayer,useless = Cat(NeuralLayer, W[index], ThresholdSigns[index], ThresholdValues[index],0)
+                    NeuralLayer,useless = Cat(NeuralLayer, W[index], MembranThresholds[index], MembranPotentials[index],0)
             for i, w in enumerate(Wc):
                 W[i] = np.copy(w)
             RealOutput = np.argmax(TestLabels[inpIndex])
             PredictedOutput = np.argmax(NeuralLayer)
             if RealOutput == PredictedOutput:
                 true += 1
             Acc = true / len(TestLabels)
@@ -636,25 +636,25 @@
             print(Fore.MAGENTA + '\nTotal Test Accuracy: ' ,Acc, '\n' + Style.RESET_ALL)
         
         elif Acc <= 0.6:
             print(Fore.RED+ '\nTotal Test Accuracy: ' ,Acc, '\n' + Style.RESET_ALL)   
     
     except:
         
-        print(Fore.RED + "ERROR: Testing model parameters like 'Layers' 'ThresholdCounts' must be same as trained model. Check parameters. Are you sure weights are loaded ? from: TestPLAN" + infoTestModel + Style.RESET_ALL)
+        print(Fore.RED + "ERROR: Testing model parameters like 'Layers' 'MembranCounts' must be same as trained model. Check parameters. Are you sure weights are loaded ? from: TestPLAN" + infoTestModel + Style.RESET_ALL)
         return 'e'
    
     return W,TestPredictions,Acc
 
 def SavePLAN(ModelName,
              ModelType,
              Layers,
              ClassCount,
-             ThresholdSigns,
-             ThresholdValues,
+             MembranThresholds,
+             MembranPotentials,
              Normalizations,
              Activations,
              TestAcc,
              LogType,
              WeightsType,
              WeightsFormat,
              ModelPath,
@@ -665,16 +665,16 @@
     Function to save a deep learning model.
 
     Arguments:
     ModelName (str): Name of the model.
     ModelType (str): Type of the model.(options: PLAN)
     Layers (list): List containing 'fex' and 'cat' layers.
     ClassCount (int): Number of classes.
-    ThresholdSigns (list): List containing threshold signs.
-    ThresholdValues (list): List containing threshold values.
+    MembranThresholds (list): List containing MEMBRAN THRESHOLDS.
+    MembranPotentials (list): List containing MEMBRAN POTENTIALS.
     DoNormalization (str): is that normalized data ? 'y' or 'n'.
     Activations (list): List containing activation functions for each layer.
     TestAcc (float): Test accuracy of the model.
     LogType (str): Type of log to save (options: 'csv', 'txt', 'hdf5').
     WeightsType (str): Type of weights to save (options: 'txt', 'npy', 'mat').
     WeightFormat (str): Format of the weights (options: 'd', 'f', 'raw').
     ModelPath (str): Path where the model will be saved. For example: C:/Users/beydili/Desktop/denemePLAN/
@@ -714,16 +714,16 @@
     from scipy import io
     
     data = {'MODEL NAME': ModelName,
             'MODEL TYPE': ModelType,
             'LAYERS': Layers,
             'LAYER COUNT': len(Layers),
             'CLASS COUNT': ClassCount,
-            'THRESHOLD SIGNS': ThresholdSigns,
-            'THRESHOLD VALUES': ThresholdValues,
+            'MEMBRAN THRESHOLDS': MembranThresholds,
+            'MEMBRAN POTENTIALS': MembranPotentials,
             'NORMALIZATION': Normalizations,
             'ACTIVATIONS': Activations,
             'NEURON COUNT': NeuronCount,
             'SYNAPSE COUNT': SynapseCount,
             'TEST ACCURACY': TestAcc,
             'SAVE DATE': datetime.now(),
             'WEIGHTS TYPE': WeightsType,
@@ -831,15 +831,15 @@
 
    Arguments:
    ModelName (str): Name of the model.
    ModelPath (str): Path where the model is saved.
    LogType (str): Type of log to load (options: 'csv', 'txt', 'hdf5').
 
    Returns:
-   lists: W(list[num]), Layers, ThresholdSigns, ThresholdValues, Normalization,Activations
+   lists: W(list[num]), Layers, MembranThresholds, MembranPotentials, Normalization,Activations
     """
    pass
 
     
    import pandas as pd
    import scipy.io as sio
    
@@ -858,16 +858,16 @@
    except:
        print(Fore.RED + "ERROR: Model Path error. Accaptable form: 'C:/Users/hasancanbeydili/Desktop/denemePLAN/' from: LoadPLAN" + infoLoadPLAN + Style.RESET_ALL)
 
    ModelName = str(df['MODEL NAME'].iloc[0])
    Layers = df['LAYERS'].tolist()
    LayerCount = int(df['LAYER COUNT'].iloc[0])
    ClassCount = int(df['CLASS COUNT'].iloc[0])
-   ThresholdSigns = df['THRESHOLD SIGNS'].tolist()
-   ThresholdValues = df['THRESHOLD VALUES'].tolist()
+   MembranThresholds = df['MEMBRAN THRESHOLDS'].tolist()
+   MembranPotentials = df['MEMBRAN POTENTIALS'].tolist()
    Normalizations = df['NORMALIZATION'].tolist()
    Activations = df['ACTIVATIONS'].tolist()
    NeuronCount = int(df['NEURON COUNT'].iloc[0])
    SynapseCount = int(df['SYNAPSE COUNT'].iloc[0])
    TestAcc = int(df['TEST ACCURACY'].iloc[0])
    ModelType = str(df['MODEL TYPE'].iloc[0])
    WeightType = str(df['WEIGHTS TYPE'].iloc[0])
@@ -884,30 +884,30 @@
            W[i] = np.load(ModelPath + ModelName + str(i+1) + 'w.npy')
    elif WeightType == 'mat':
        for i in range(LayerCount):  
            W[i] = sio.loadmat(ModelPath + ModelName + str(i+1) + 'w.mat')
    else:
         raise ValueError(Fore.RED + "Incorrect weight type value. Value must be 'txt', 'npy' or 'mat' from: LoadPLAN."  + infoLoadPLAN + Style.RESET_ALL)
    print(Fore.GREEN + "Model loaded succesfully" + Style.RESET_ALL)     
-   return W,Layers,ThresholdSigns,ThresholdValues,Normalizations,Activations,df
+   return W,Layers,MembranThresholds,MembranPotentials,Normalizations,Activations,df
 
 def PredictFromDiscPLAN(Input,ModelName,ModelPath,LogType):
     infoPredictFromDİscPLAN = """
     Function to make a prediction using a divided pruning deep learning neural network (PLAN).
 
     Arguments:
     Input (list or ndarray): Input data for the model (single vector or single matrix).
     ModelName (str): Name of the model.
     ModelPath (str): Path where the model is saved.
     LogType (str): Type of log to load (options: 'csv', 'txt', 'hdf5').
 
     Returns:
     ndarray: Output from the model.
     """
-    W,Layers,ThresholdSigns,ThresholdValues,Normalizations,Activations = LoadPLAN(ModelName,ModelPath,
+    W,Layers,MembranThresholds,MembranPotentials,Normalizations,Activations = LoadPLAN(ModelName,ModelPath,
                                                                                   LogType)[0:6]
     Wc = [0] * len(W)
     for i, w in enumerate(W):
         Wc[i] = np.copy(w)
     try:
         NeuralLayer = Input
         NeuralLayer = np.array(NeuralLayer)
@@ -920,39 +920,39 @@
             elif Activations[index] == 'sigmoid':
                 NeuralLayer = Sigmoid(NeuralLayer)
             elif Activations[index] == 'softmax':
                 NeuralLayer = Softmax(NeuralLayer)
                                 
             if Layers[index] == 'fex':
                 NeuralLayer,useless = Fex(NeuralLayer, W[index],
-                                          ThresholdSigns[index],
-                                          ThresholdValues[index])
+                                          MembranThresholds[index],
+                                          MembranPotentials[index])
             if Layers[index] == 'cat':
                 NeuralLayer,useless = Cat(NeuralLayer, W[index],
-                                          ThresholdSigns[index],
-                                          ThresholdValues[index],
+                                          MembranThresholds[index],
+                                          MembranPotentials[index],
                                           0)
     except:
        print(Fore.RED + "ERROR: The input was probably entered incorrectly. from: PredictFromDiscPLAN"  + infoPredictFromDİscPLAN + Style.RESET_ALL)
        return 'e'
     for i, w in enumerate(Wc):
         W[i] = np.copy(w)
     return NeuralLayer
 
 
-def PredictFromRamPLAN(Input,Layers,ThresholdSigns,ThresholdValues,Normalizations,Activations,W):
+def PredictFromRamPLAN(Input,Layers,MembranThresholds,MembranPotentials,Normalizations,Activations,W):
     infoPredictFromRamPLAN = """
     Function to make a prediction using a pruning learning artificial neural network (PLAN)
     from weights and parameters stored in memory.
 
     Arguments:
     Input (list or ndarray): Input data for the model (single vector or single matrix).
     Layers (list): Number and types of layers.
-    ThresholdSigns (list): Threshold signs.
-    ThresholdValues (list): Threshold values.
+    MembranThresholds (list): MEMBRAN THRESHOLDS.
+    MembranPotentials (list): MEMBRAN POTENTIALS.
     DoNormalization (str): Whether to normalize ('y' or 'n').
     Activations (list): Activation functions for each layer.
     W (list of ndarrays): Weights of the model.
 
     Returns:
     ndarray: Output from the model.
     """
@@ -972,20 +972,20 @@
             elif Activations[index] == 'sigmoid':
                 NeuralLayer = Sigmoid(NeuralLayer)
             elif Activations[index] == 'softmax':
                 NeuralLayer = Softmax(NeuralLayer)
                                 
             if Layers[index] == 'fex':
                 NeuralLayer,useless = Fex(NeuralLayer, W[index],
-                                          ThresholdSigns[index],
-                                          ThresholdValues[index])
+                                          MembranThresholds[index],
+                                          MembranPotentials[index])
             if Layers[index] == 'cat':
                 NeuralLayer,useless = Cat(NeuralLayer, W[index],
-                                          ThresholdSigns[index],
-                                          ThresholdValues[index],0)
+                                          MembranThresholds[index],
+                                          MembranPotentials[index],0)
     except:
         print(Fore.RED + "ERROR: Unexpected input or wrong model parameters from: PredictFromRamPLAN."  + infoPredictFromRamPLAN + Style.RESET_ALL)
         return 'e'
     for i, w in enumerate(Wc):
         W[i] = np.copy(w)
     return NeuralLayer
```

