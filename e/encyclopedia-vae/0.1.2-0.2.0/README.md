# Comparing `tmp/encyclopedia_vae-0.1.2.tar.gz` & `tmp/encyclopedia_vae-0.2.0.tar.gz`

## Comparing `encyclopedia_vae-0.1.2.tar` & `encyclopedia_vae-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,42 @@
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/.python-version
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/Changelog.md
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/ruff.toml
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/.github/workflows/lint.yml
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/configs/bbvae.yaml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/configs/betatc_vae.yaml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/configs/cvae.yaml
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/configs/vae.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/__init__.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/cli.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/types_helpers.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/data/lit_celeba.py
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/lit_models/lit_vae.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/losses/__init__.py
--rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/losses/losses.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/models/__init__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/models/base.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/models/beta_vae.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/models/betatc_vae.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/models/cvae.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/models/vanilla_vae.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/modules/__init__.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/modules/decoder.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/modules/encoder.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/modules/residual.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/modules/vectorquantizer.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/tests/test_betatcvae.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/tests/test_betavae.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/tests/test_cvae.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/tests/test_vae.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/.gitignore
--rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/LICENSE.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/README.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/.python-version
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/Changelog.md
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/ruff.toml
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/configs/bbvae.yaml
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/configs/betatc_vae.yaml
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/configs/config_cli.yml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/configs/cvae.yaml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/configs/data_litceleb.yml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/configs/model_vae.yml
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/configs/vae.yaml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/cli.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/types_helpers.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/data/lit_celeba.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/data/lit_oxfordiitpet.py
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/lit_models/lit_vae.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/losses/__init__.py
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/losses/losses.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/models/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/models/base.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/models/beta_vae.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/models/betatc_vae.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/models/cvae.py
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/models/vanilla_vae.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/modules/__init__.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/modules/decoder.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/modules/encoder.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/modules/residual.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/encyclopedia_vae/modules/vectorquantizer.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/tests/test_betatcvae.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/tests/test_betavae.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/tests/test_cvae.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/tests/test_vae.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/README.md
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 encyclopedia_vae-0.2.0/PKG-INFO
```

### Comparing `encyclopedia_vae-0.1.2/.pre-commit-config.yaml` & `encyclopedia_vae-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.2/.github/workflows/lint.yml` & `encyclopedia_vae-0.2.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.2/.github/workflows/publish.yml` & `encyclopedia_vae-0.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.2/.github/workflows/test.yml` & `encyclopedia_vae-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.2/encyclopedia_vae/data/lit_celeba.py` & `encyclopedia_vae-0.2.0/encyclopedia_vae/data/lit_celeba.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.2/encyclopedia_vae/lit_models/lit_vae.py` & `encyclopedia_vae-0.2.0/encyclopedia_vae/lit_models/lit_vae.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.2/encyclopedia_vae/models/__init__.py` & `encyclopedia_vae-0.2.0/encyclopedia_vae/models/__init__.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.2/encyclopedia_vae/models/base.py` & `encyclopedia_vae-0.2.0/encyclopedia_vae/models/base.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.2/encyclopedia_vae/models/betatc_vae.py` & `encyclopedia_vae-0.2.0/encyclopedia_vae/models/betatc_vae.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,38 @@
+"""Module for the BetaTC VAE implementation."""
+
 import torch
 from torch import nn
 
 from encyclopedia_vae.losses import loss_function_betatc
 from encyclopedia_vae.models.vanilla_vae import VanillaVAE
 from encyclopedia_vae.modules import (
     build_encoder,
 )
-from encyclopedia_vae.types_helpers import EncoderReturn, ForwardReturn
+from encyclopedia_vae.types_helpers import OutputEncoder, OutputModel
 
 
 class BetaTCVAE(VanillaVAE):
+    """Implementation of BetaTC VAE model.
+
+    Subclass the bare VAE model that is VanillaVAE.
+
+    Attributes
+    ----------
+    beta: int
+        beta arg, by default 4.
+    anneal_steps: int, optional
+        number of anneal steps, by default 200
+
+    Methods
+    -------
+    loss(output_model, kld_weight)
+        the loss function for the BetaVAE model.
+    """
+
     def __init__(
         self,
         in_channels: int,
         latent_dim: int,
         hidden_dims: list = [32, 32, 32, 32],
         mid_inflate: int = 4,
         mid_dim: int = 256 * 2,
@@ -41,39 +60,53 @@
             in_channels=in_channels, hidden_dims=hidden_dims, kernel_size=4
         )
 
         self.fc = nn.Linear(hidden_dims[-1] * 16, 256)
         self.fc_mu = nn.Linear(256, latent_dim)
         self.fc_var = nn.Linear(256, latent_dim)
 
-    def encode(self, input: torch.tensor) -> EncoderReturn:
-        """
-        Encodes the input by passing through the encoder network
-        and returns the latent codes.
-        :param input: (torch.tensor) Input tensor to encoder [N x C x H x W]
-        :return: (torch.tensor) List of latent codes
+    def encode(self, input: torch.tensor) -> OutputEncoder:
+        """Encode the input and returns the latent codes.
+
+        Parameters
+        ----------
+        input: torch.tensor
+            Input tensor to encoder [N x C x H x W]
+
+        Returns
+        -------
+        OutputEncoder
+            contains mu, log_var and pre-latent tensors.
         """
         result = self.encoder(input)
         result = self.flatten(result)
 
         result = self.fc(result)
         mu = self.fc_mu(result)
         log_var = self.fc_var(result)
 
-        return EncoderReturn(mu=mu, log_var=log_var, pre_latents=result)
+        return OutputEncoder(mu=mu, log_var=log_var, pre_latents=result)
 
-    def loss(self, output_model: ForwardReturn, kld_weight) -> dict:
-        """
-        Computes the VAE loss function.
-        KL(N(\mu, \sigma), N(0, 1)) = \log \frac{1}{\sigma} + \frac{\sigma^2 + \mu^2}{2} - \frac{1}{2}
-        :param args:
-        :param kwargs:
-        :return:
-        """
+    def loss(self, output_model: OutputModel, kld_weight) -> dict:
+        """Loss function.
 
+        Wraps the encyclopedia_vae.losses.loss_function_betatc.
+
+        Parameters
+        ----------
+        output_model : OutputModel
+            _description_
+        kld_weight : float
+            _description_
+
+        Returns
+        -------
+        OutputLoss
+            _description_
+        """
         loss = loss_function_betatc(
             output_model=output_model,
             kld_weight=kld_weight,
             num_iter=self.num_iter,
             anneal_steps=self.anneal_steps,
             alpha=self.alpha,
             beta=self.beta,
```

### Comparing `encyclopedia_vae-0.1.2/encyclopedia_vae/models/cvae.py` & `encyclopedia_vae-0.2.0/encyclopedia_vae/models/cvae.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 from torch import nn
 
 from encyclopedia_vae.models.vanilla_vae import VanillaVAE
-from encyclopedia_vae.types_helpers import ForwardReturn
+from encyclopedia_vae.types_helpers import OutputModel
 
 
 class ConditionalVAE(VanillaVAE):
     def __init__(
         self,
         in_channels: int,
         num_classes: int,
@@ -22,29 +22,29 @@
         )
 
         self.img_size = img_size
 
         self.embed_class = nn.Linear(num_classes, img_size * img_size)
         self.embed_data = nn.Conv2d(in_channels, in_channels, kernel_size=1)
 
-    def forward(self, input: torch.tensor, labels: torch.tensor) -> ForwardReturn:
+    def forward(self, input: torch.tensor, labels: torch.tensor) -> OutputModel:
         y = labels.float()
         embedded_class = self.embed_class(y)
         embedded_class = embedded_class.view(
             -1, self.img_size, self.img_size
         ).unsqueeze(1)
         embedded_input = self.embed_data(input)
 
         x = torch.cat([embedded_input, embedded_class], dim=1)
         latents = self.encode(x)
         mu, log_var, _ = latents.values()
         z = self.reparametrize(mu, log_var)
 
         z = torch.cat([z, y], dim=1)
-        return ForwardReturn(
+        return OutputModel(
             output=self.decode(z), input=input, encoded=latents, latents=z
         )
 
     def sample(self, num_samples: int, labels: torch.tensor) -> torch.tensor:
         """
         Samples from the latent space and return the corresponding
         image space map.
@@ -61,9 +61,8 @@
 
     def generate(self, x: torch.tensor, labels: torch.tensor) -> torch.tensor:
         """
         Given an input image x, returns the reconstructed image
         :param x: (torch.tensor) [B x C x H x W]
         :return: (torch.tensor) [B x C x H x W]
         """
-
         return self.forward(x, labels)["output"]
```

### Comparing `encyclopedia_vae-0.1.2/encyclopedia_vae/models/vanilla_vae.py` & `encyclopedia_vae-0.2.0/encyclopedia_vae/models/vanilla_vae.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,40 @@
+"""Module for the implementation of the Vanilla VAE model."""
+
 import torch
 from einops.layers.torch import Rearrange
 from torch import nn
 
 from encyclopedia_vae.losses import loss_function
 from encyclopedia_vae.modules import (
     build_encoder,
     build_full_decoder,
 )
-from encyclopedia_vae.types_helpers import EncoderReturn, ForwardReturn, LossReturn
+from encyclopedia_vae.types_helpers import OutputEncoder, OutputLoss, OutputModel
 
 
 class VanillaVAE(nn.Module):
+    """Implementation of the classical VAE.
+
+    Attributes
+    ----------
+    latent_dim: int
+        dimension of the latent space
+    encoder: nn.Module
+        implements the Encoder part
+    full_decoder: nn.Module
+        implements the Decoder part
+    flatten: nn.Module
+        einops Rearrange layer to ease the pre process of the latent work
+    fc_mu: nn.Module
+        linear Module which "learns" the mean vector of the latents distribution
+    fc_var: nn.Module
+        linear Module which "learns" the log-var vector of the latents distribution
+    """
+
     def __init__(
         self,
         in_channels: int,
         latent_dim: int,
         latent_dim_dec: int = None,
         hidden_dims: list = [32, 64, 128, 256, 512],
         mid_inflate: int = 2,
@@ -34,83 +54,129 @@
         self.full_decoder = build_full_decoder(
             latent_dim=latent_dim_dec,
             hidden_dims=hidden_dims[::-1],
             mid_inflate=mid_inflate,
             mid_dim=mid_dim,
         )
 
-    def encode(self, input: torch.tensor) -> EncoderReturn:
-        """
-        Encodes the input by passing through the encoder network
-        and returns the latent codes.
-        :param input: (torch.tensor) Input tensor to encoder [N x C x H x W]
-        :return: (torch.tensor) List of latent codes
+    def encode(self, input: torch.tensor) -> OutputEncoder:
+        """Encode the input and returns the latent codes.
+
+        Parameters
+        ----------
+        input: torch.tensor
+            Input tensor to encoder [N x C x H x W]
+
+        Returns
+        -------
+        OutputEncoder
+            contains mu, log_var and pre-latent tensors.
         """
         result = self.encoder(input)
         result = self.flatten(result)
 
         mu = self.fc_mu(result)
         log_var = self.fc_var(result)
 
-        return EncoderReturn(mu=mu, log_var=log_var, pre_latents=result)
+        return OutputEncoder(mu=mu, log_var=log_var, pre_latents=result)
 
     def decode(self, z: torch.tensor) -> torch.tensor:
-        """
-        Maps the given latent codes
-        onto the image space.
-        :param z: (torch.tensor) [B x D]
-        :return: (torch.tensor) [B x C x H x W]
+        """Decode the given latent codes onto the image space.
+
+        Parameters
+        ----------
+        z: torch.tensor
+            tensor of latents, of shape [B x D]
+
+        Returns
+        -------
+        torch.tensor
+            tensor of shape[B x C x H x W]
         """
         result = self.full_decoder(z)
         return result
 
     def reparametrize(self, mu: torch.tensor, logvar: torch.tensor) -> torch.tensor:
-        """
-        Reparameterization trick to sample from N(mu, var) from
-        N(0,1).
-        :param mu: (torch.tensor) Mean of the latent Gaussian [B x D]
-        :param logvar: (torch.tensor) Standard deviation of the latent Gaussian [B x D]
-        :return: (torch.tensor) [B x D]
+        """Implement the reparameterization trick.
+
+        The reparametrization trick to sample from N(mu, var) from N(0,1).
+
+        Parameters
+        ----------
+        mu: torch.tensor
+            Mean of the latent Gaussian [B x D]
+        logvar: torch.tensor
+            Standard deviation of the latent Gaussian [B x D]
+
+        Returns
+        -------
+        torch.tensor
+            tensor of shape [B x D]
         """
         std = torch.exp(0.5 * logvar)
         eps = torch.randn_like(std)
         return eps * std + mu
 
-    def forward(self, input: torch.tensor) -> ForwardReturn:
+    def forward(self, input: torch.tensor) -> OutputModel:
+        """Forward function.
+
+        Parameters
+        ----------
+        input : torch.tensor
+            tensor of shape [B C H W]
+
+        Returns
+        -------
+        OutputModel
+            contains output, input, various latents tensors.
+        """
         latents = self.encode(input)
         mu, log_var, _ = latents.values()
         z = self.reparametrize(mu, log_var)
-        return ForwardReturn(
+        return OutputModel(
             output=self.decode(z), input=input, encoded=latents, latents=z
         )
 
-    def loss(self, output_model: ForwardReturn, kld_weight: float) -> LossReturn:
-        """Computes the VAE loss function.
+    def loss(self, output_model: OutputModel, kld_weight: float) -> OutputLoss:
+        """Compute the VAE loss function.
 
-        KL(N(\mu, \sigma), N(0, 1)) = \log \frac{1}{\sigma} + \frac{\sigma^2 + \mu^2}{2} - \frac{1}{2}
-        :param args:
-        :param kwargs:
-        :return:
-        """
+        Wraps the loss_function defined in the losses module.
 
+        Parameters
+        ----------
+        output_model: OutputModel
+            the output of the full model.
+        kld_weight: float
+            the weight for the KLD loss term.
+        """
         return loss_function(output_model, kld_weight)
 
     def sample(self, num_samples: int) -> torch.tensor:
-        """
-        Samples from the latent space and return the corresponding
-        image space map.
-        :param num_samples: (Int) Number of samples
-        :param current_device: (Int) Device to run the model
-        :return: (torch.tensor)
+        """Sample images from the latent space.
+
+        Parameters
+        ----------
+        num_samples: int
+            Number of samples
+
+        Returns
+        -------
+        torch.tensor
         """
         z = torch.randn(num_samples, self.latent_dim)
         samples = self.decode(z)
         return samples
 
     def generate(self, x: torch.tensor) -> torch.tensor:
-        """
-        Given an input image x, returns the reconstructed image
-        :param x: (torch.tensor) [B x C x H x W]
-        :return: (torch.tensor) [B x C x H x W]
-        """
+        """Return the reconstructed image from tensor x.
 
+        Parameters
+        ----------
+        x: torch.tensor
+            input tensor of shape [B x C x H x W]
+
+        Returns
+        -------
+        torch.tensor
+            generated tensor from the model, of shape [B x C x H x W]
+        """
         return self.forward(x)["output"]
```

### Comparing `encyclopedia_vae-0.1.2/encyclopedia_vae/modules/vectorquantizer.py` & `encyclopedia_vae-0.2.0/encyclopedia_vae/modules/vectorquantizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 from torch import nn
-from torch.nn import functional as F
+from torch.nn import functional
 
 
 class VectorQuantizer(nn.Module):
     """
     Reference:
     [1] https://github.com/deepmind/sonnet/blob/v2/sonnet/src/nets/vqvae.py
     """
@@ -43,16 +43,16 @@
         # Quantize the latents
         quantized_latents = torch.matmul(
             encoding_one_hot, self.embedding.weight
         )  # [BHW, D]
         quantized_latents = quantized_latents.view(latents_shape)  # [B x H x W x D]
 
         # Compute the VQ Losses
-        commitment_loss = F.mse_loss(quantized_latents.detach(), latents)
-        embedding_loss = F.mse_loss(quantized_latents, latents.detach())
+        commitment_loss = functional.mse_loss(quantized_latents.detach(), latents)
+        embedding_loss = functional.mse_loss(quantized_latents, latents.detach())
 
         vq_loss = commitment_loss * self.beta + embedding_loss
 
         # Add the residue back to the latents
         quantized_latents = latents + (quantized_latents - latents).detach()
 
         return quantized_latents.permute(
```

### Comparing `encyclopedia_vae-0.1.2/tests/test_betatcvae.py` & `encyclopedia_vae-0.2.0/tests/test_betatcvae.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.2/tests/test_betavae.py` & `encyclopedia_vae-0.2.0/tests/test_betavae.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.2/tests/test_cvae.py` & `encyclopedia_vae-0.2.0/tests/test_cvae.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.2/tests/test_vae.py` & `encyclopedia_vae-0.2.0/tests/test_vae.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.2/LICENSE.md` & `encyclopedia_vae-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.2/README.md` & `encyclopedia_vae-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.2/pyproject.toml` & `encyclopedia_vae-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 [project]
 name = "encyclopedia-vae"
-version = "0.1.2"
+version = "0.2.0"
 description = "Add your description here"
 authors = [
     { name = "BaptisteMorisse", email = "bmorisse.pro@proton.me" }
 ]
 dependencies = [
     "torch>=2.3.0",
     "lightning[pytorch-extra]>=2.2.4",
     "einops>=0.8.0",
     "torchsummary>=1.5.1",
+    "jsonargparse[signatures]>=4.28.0",
+    # "torchvision>=0.18.0",
 ]
 readme = "README.md"
 requires-python = ">= 3.9"
 
+[project.optional-dependencies]
+examples = [
+    "torchvision>=0.18.0",
+]
+
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
```

### Comparing `encyclopedia_vae-0.1.2/PKG-INFO` & `encyclopedia_vae-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.3
 Name: encyclopedia-vae
-Version: 0.1.2
+Version: 0.2.0
 Summary: Add your description here
 Author-email: BaptisteMorisse <bmorisse.pro@proton.me>
 License-File: LICENSE.md
 Requires-Python: >=3.9
 Requires-Dist: einops>=0.8.0
+Requires-Dist: jsonargparse[signatures]>=4.28.0
 Requires-Dist: lightning[pytorch-extra]>=2.2.4
 Requires-Dist: torch>=2.3.0
 Requires-Dist: torchsummary>=1.5.1
+Provides-Extra: examples
+Requires-Dist: torchvision>=0.18.0; extra == 'examples'
 Description-Content-Type: text/markdown
 
 # A modular, easy to use Encyclopedia of VAE
 
 ** STILL WORK IN PROGRESS **
 
 This project aims at working from the repo Pytorch-VAE and upgrading it (a lot).
```

