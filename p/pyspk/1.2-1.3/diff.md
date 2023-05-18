# Comparing `tmp/pyspk-1.2.tar.gz` & `tmp/pyspk-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspk-1.2.tar", last modified: Fri Mar 24 10:23:49 2023, max compression
+gzip compressed data, was "pyspk-1.3.tar", last modified: Thu May 18 08:48:02 2023, max compression
```

## Comparing `pyspk-1.2.tar` & `pyspk-1.3.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-03-24 10:23:49.868608 pyspk-1.2/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     7326 2022-09-13 12:12:10.000000 pyspk-1.2/LICENSE.md
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       25 2022-09-14 12:27:24.000000 pyspk-1.2/MANIFEST.in
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     8607 2023-03-24 10:23:49.868399 pyspk-1.2/PKG-INFO
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     8086 2022-11-18 11:42:02.000000 pyspk-1.2/README.md
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-03-24 10:23:49.866411 pyspk-1.2/pyspk/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     6148 2022-09-24 18:18:43.000000 pyspk-1.2/pyspk/.DS_Store
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       20 2022-09-13 12:12:10.000000 pyspk-1.2/pyspk/__init__.py
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-03-24 10:23:49.867999 pyspk-1.2/pyspk/__pycache__/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      156 2022-09-25 14:31:25.000000 pyspk-1.2/pyspk/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     2083 2022-09-25 14:31:25.000000 pyspk-1.2/pyspk/__pycache__/fit_vals.cpython-39.pyc
--rw-r--r--   0 jaimesalcido   (501) staff       (20)    14636 2022-11-04 10:54:05.000000 pyspk-1.2/pyspk/__pycache__/model.cpython-39.pyc
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     4114 2023-03-24 10:17:38.000000 pyspk-1.2/pyspk/fit_vals.py
--rw-r--r--   0 jaimesalcido   (501) staff       (20)    16276 2022-11-18 10:46:25.000000 pyspk-1.2/pyspk/model.py
--rw-r--r--   0 jaimesalcido   (501) staff       (20)   180313 2022-09-24 07:34:27.000000 pyspk-1.2/pyspk/stat_errors_200.csv
--rw-r--r--   0 jaimesalcido   (501) staff       (20)   179350 2022-09-24 07:36:40.000000 pyspk-1.2/pyspk/stat_errors_500.csv
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-03-24 10:23:49.867477 pyspk-1.2/pyspk.egg-info/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     8607 2023-03-24 10:23:49.000000 pyspk-1.2/pyspk.egg-info/PKG-INFO
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      427 2023-03-24 10:23:49.000000 pyspk-1.2/pyspk.egg-info/SOURCES.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)        1 2023-03-24 10:23:49.000000 pyspk-1.2/pyspk.egg-info/dependency_links.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       12 2023-03-24 10:23:49.000000 pyspk-1.2/pyspk.egg-info/requires.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)        6 2023-03-24 10:23:49.000000 pyspk-1.2/pyspk.egg-info/top_level.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       38 2023-03-24 10:23:49.868650 pyspk-1.2/setup.cfg
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      807 2023-03-24 10:19:40.000000 pyspk-1.2/setup.py
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-05-18 08:48:02.905345 pyspk-1.3/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     7326 2022-09-13 12:12:10.000000 pyspk-1.3/LICENSE.md
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       25 2022-09-14 12:27:24.000000 pyspk-1.3/MANIFEST.in
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     9087 2023-05-18 08:48:02.905172 pyspk-1.3/PKG-INFO
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     8566 2023-05-18 08:41:38.000000 pyspk-1.3/README.md
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-05-18 08:48:02.902318 pyspk-1.3/pyspk/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     6148 2022-09-24 18:18:43.000000 pyspk-1.3/pyspk/.DS_Store
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       20 2022-09-13 12:12:10.000000 pyspk-1.3/pyspk/__init__.py
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-05-18 08:48:02.904863 pyspk-1.3/pyspk/__pycache__/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      156 2023-04-26 10:36:22.000000 pyspk-1.3/pyspk/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      156 2022-09-25 14:31:25.000000 pyspk-1.3/pyspk/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     2169 2023-04-26 10:37:02.000000 pyspk-1.3/pyspk/__pycache__/fit_vals.cpython-38.pyc
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     2083 2022-09-25 14:31:25.000000 pyspk-1.3/pyspk/__pycache__/fit_vals.cpython-39.pyc
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)    18870 2023-05-02 10:10:08.000000 pyspk-1.3/pyspk/__pycache__/model.cpython-38.pyc
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)    14636 2022-11-04 10:54:05.000000 pyspk-1.3/pyspk/__pycache__/model.cpython-39.pyc
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     4114 2023-03-24 10:17:38.000000 pyspk-1.3/pyspk/fit_vals.py
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)    16276 2023-05-12 14:14:32.000000 pyspk-1.3/pyspk/model.py
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)   180313 2022-09-24 07:34:27.000000 pyspk-1.3/pyspk/stat_errors_200.csv
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)   179350 2022-09-24 07:36:40.000000 pyspk-1.3/pyspk/stat_errors_500.csv
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-05-18 08:48:02.903538 pyspk-1.3/pyspk.egg-info/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     9087 2023-05-18 08:48:02.000000 pyspk-1.3/pyspk.egg-info/PKG-INFO
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      550 2023-05-18 08:48:02.000000 pyspk-1.3/pyspk.egg-info/SOURCES.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)        1 2023-05-18 08:48:02.000000 pyspk-1.3/pyspk.egg-info/dependency_links.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       12 2023-05-18 08:48:02.000000 pyspk-1.3/pyspk.egg-info/requires.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)        6 2023-05-18 08:48:02.000000 pyspk-1.3/pyspk.egg-info/top_level.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       38 2023-05-18 08:48:02.905382 pyspk-1.3/setup.cfg
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      807 2023-05-18 08:45:27.000000 pyspk-1.3/setup.py
```

### Comparing `pyspk-1.2/LICENSE.md` & `pyspk-1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyspk-1.2/PKG-INFO` & `pyspk-1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pyspk
-Version: 1.2
-Summary: Python package to predict the suppression of the total matter power spectrum due to baryonic physics
-Home-page: https://github.com/jemme07/pyspk
-Author: Jaime Salcido
-Author-email: j.salcidonegrete@ljmu.ac.uk
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # py-SP(k) - A hydrodynamical simulation-based model for the impact of baryon physics on the non-linear matter power spectrum
                           _____ ____   ____   _ 
         ____  __  __     / ___// __ \_/_/ /__| |
        / __ \/ / / /_____\__ \/ /_/ / // //_// /
       / /_/ / /_/ /_____/__/ / ____/ // ,<  / / 
      / .___/\__, /     /____/_/   / //_/|_|/_/  
     /_/    /____/                 |_|    /_/    
@@ -61,23 +48,23 @@
 fb_pivot = 10 ** 13.5
 
 k, sup = spk.sup_model(SO=200, z=z, fb_a=fb_a, fb_pow=fb_pow, fb_pivot=fb_pivot)
 ```
 
 ### Method 2: Redshift-dependent power-law fit to the $f_b$ - $M_\mathrm{halo}$ relation. 
 
-For the mass range that can be relatively well probed in current X-ray and Sunyaev-Zel'dovich effect observations (roughly $10^{13} \leq M_{500c} [\mathrm{M}_ \odot] \leq 10^{15}$), the total baryon fraction of haloes can be roughly approximated by a power-law with constant slope (e.g. Mulroy et al. 2019; Akino et al. 2022). Akino et al. 2022 determined the of the baryon budget for X-ray-selected galaxy groups and clusters using weak-lensing mass measurements. They provide a parametric redshift-dependent power-law fit to the gas mass - halo mass and stellar mass - halo mass relations, finding very little redshift evolution. 
+For the mass range that can be relatively well probed in current X-ray and Sunyaev-Zel'dovich effect observations (roughly $10^{13} \leq M_{500c} [\mathrm{M}_ \odot] \leq 10^{15}$), the total baryon fraction of haloes can be roughly approximated by a power-law with constant slope (e.g. Mulroy et al. 2019; Akino et al. 2022). Akino et al. (2022) determined the of the baryon budget for X-ray-selected galaxy groups and clusters using weak-lensing mass measurements. They provide a parametric redshift-dependent power-law fit to the gas mass - halo mass and stellar mass - halo mass relations, finding very little redshift evolution. 
 
-We implemented a modified version of the functional form presented in Akino et al. 2022, to fit the total $f_b$ - $M_\mathrm{halo}$ relation as follows:
+We implemented a modified version of the functional form presented in Akino et al. (2022), to fit the total $f_b$ - $M_\mathrm{halo}$ relation as follows:
 
 $$f_b/(\Omega_b/\Omega_m)= \left(\frac{0.1658}{\Omega_b/\Omega_m}\right) \left(\frac{e^\alpha}{100}\right) \left(\frac{M_{500c}}{10^{14} \mathrm{M}_ \odot}\right)^{\beta - 1} \left(\frac{E(z)}{E(0.3)}\right)^{\gamma},$$
 
 where $\alpha$ sets the power-law normalisation, $\beta$ sets power-law slope, $\gamma$ provides the redshift dependence and $E(z)$ is the usual dimensionless Hubble parameter. For simplicity, we use the cosmology implementation of `astropy` to specify the cosmological parameters in py-SP(k).
 
-Note that this power-law has a normalisation that is redshift dependent, while the the slop is constant in redshift. While this provides a less flexible approach compared with Methods 1 (simple power-law) and Method 3 (binned data), we find that this parametrisation agrees well with our simulations up to redshift $z=1$, which is the redshift range proved by Akino et al. 2022. For higher redshifts, we find that simulations require a mass-dependent slope, especially at the lower mass range required to predict the suppression of the total matter power spectrum at such redshifts. 
+Note that this power-law has a normalisation that is redshift dependent, while the the slope is constant in redshift. While this provides a less flexible approach compared with Methods 1 (simple power-law) and Method 3 (binned data), we find that this parametrisation provides a reasonable agreement with our simulations up to redshift $z=1$, which is the redshift range proved by Akino et al. (2022). For higher redshifts, we find that simulations require a mass-dependent slope, especially at the lower mass range required to predict the suppression of the total matter power spectrum at such redshifts. 
 
 In the following example we use the redshift-dependent power-law fit parameters with a flat LambdaCDM cosmology. Note that any `astropy` cosmology could be used instead.
 
 ```
 import pyspk.model as spk
 from astropy.cosmology import FlatLambdaCDM
 
@@ -93,70 +80,57 @@
 z = 0.5
 
 k, sup = spk.sup_model(SO=500, z=z, alpha=alpha, beta=beta, gamma=gamma, cosmo=cosmo)
 ```
 
 ### Method 3: Binned data for the $f_b$ - $M_\mathrm{halo}$ relation. 
 
-The final, and most flexible method is to provide py-SP(k) with the baryon fraction binned in bins of halo mass. This could be, for example, obtained from observational constraints, measured directly form simulations, or sampled from a predefined distribution or functional form. For an example using data obtained from the BAHAMAS simulations ([McCarthy et al. 2017](https://academic.oup.com/mnras/article/465/3/2936/2417021)), please refer to the [examples](https://github.com/jemme07/pyspk/blob/main/examples/pySPk_Examples.ipynb) provided. 
+The final, and most flexible method is to provide py-SP(k) with the baryon fraction binned in bins of halo mass. This could be, for example, obtained from observational constraints, measured directly form simulations, or sampled from a predefined distribution or functional form. For an example using data obtained from the BAHAMAS simulations (McCarthy et al. 2017), please refer to the [examples](https://github.com/jemme07/pyspk/blob/main/examples/pySPk_Examples.ipynb) provided. 
 
 
 ## Priors
 
-While py-SP(k) was calibrated using a wide range of sub-grid feedback parameters, some applications may require a more limited range of baryon fractions that encompass current observational constraints. For such applications, we used the gas mass - halo mass and stellar mass - halo mass constraints from Table 5 in Akino et al. 2022, and find the subset of simulations from our 400 models that agree with the inferred baryon budget at redshift $z=0.1$. We note that we constrained our simulations to within a normalisation of $\pm 3 \times \sigma$ at $M_{500c} = 10^{14} \mathrm{M}_ \odot$. 
-
-Using the simulations that fall within these constraints, we can impose observational priors for the redshift-dependent power-law fitting parameters for the $f_b$ - $M_\mathrm{halo}$ relation in Method 3 as follows:
-
-| Parameter   | Description        | Prior           |
-| ----------- | ------------------ | --------------- |
-| $\alpha$    | Normaliasation     | G(4.189, 0.066) |
-| $\beta$     | Slope              | G(1.273, 0.044) |
-| $\gamma$    | Redshift evolution | G(0.298, 0.063) |
+While py-SP(k) was calibrated using a wide range of sub-grid feedback parameters, some applications may require a more limited range of baryon fractions that encompass current observational constraints. For such applications, we used the gas mass - halo mass and stellar mass - halo mass constraints from the fits in Table 5 in Akino et al. (2022), and find the subset of simulations from our 400 models that agree to within $\pm 2$ or $3 \times \sigma$ of the inferred baryon budget at redshift $z=0.1$. We note that for our simulations, we include all stellar and gas particles within a spherical overdensity radius. Hence, in order to make reasonable comparisons with the fits in Akino et al. (2022), we included an additional 15\% contribution to the total stellar masses from the contribution of blue galaxies, and 30\% additional stellar mass to the brightest cluster galaxies (BCGs) to account for the diffuse intracluster light (ICL, see Akino et al. 2022). 
 
-where G(x, y) is a Gaussian distribution with center x and width y.
+We utilised the simulations satisfying these restrictions to determine the redshift-dependent power-law parameters for the $f_b$ - $M_\mathrm{halo}$ relation up to redshift $z=1$ (Method 2), and then utilised these parameters to infer suitable priors. We limited the fitting range to $6 \times 10^{12} \leq M_{500c} [\mathrm{M}_ \odot] \leq 10^{14}$. 
 
-A less conservative approach could be to use a flat priors over the entire range of parameters fitted to simulations that fall within Akino et al. 2022 these constraints:
+Priors inferred from simulations that fall within $\pm 2 \times \sigma$ of the inferred baryon budget:
 
 | Parameter   | Description        | Prior           |
 | ----------- | ------------------ | --------------- |
-| $\alpha$    | Normaliasation     | U(4.060, 4.306) |
-| $\beta$     | Slope              | U(1.199, 1.347) |
-| $\gamma$    | Redshift evolution | U(0.159, 0.414) |
+| $\alpha$    | Normaliasation     | $\mathcal{N}$(4.16, 0.07) |
+| $\beta$     | Slope              | $\mathcal{N}$(1.20, 0.05) |
+| $\gamma$    | Redshift evolution | $\mathcal{N}$(0.39, 0.09) |
 
-where U(x, y) is a uniform distribution over [x, y]. 
+where $\mathcal{N}(\mu,\sigma)$ is a Gaussian distribution with mean $\mu$ and standard deviation $\sigma$.
 
-Finally, the full range of fitted parameters spanned by our simulations, regardless of whether or not they agree with observational constraints is:
+Priors inferred from simulations that fall within $\pm 3 \times \sigma$ of the inferred baryon budget:
 
 | Parameter   | Description        | Prior           |
 | ----------- | ------------------ | --------------- |
-| $\alpha$    | Normaliasation     | U(3.060, 4.508) |
-| $\beta$     | Slope              | U(0.989, 1.620) |
-| $\gamma$    | Redshift evolution | U(0.046, 0.631) |
+| $\alpha$    | Normaliasation     | $\mathcal{N}$(4.18, 0.12) |
+| $\beta$     | Slope              | $\mathcal{N}$(1.26, 0.08) |
+| $\gamma$    | Redshift evolution | $\mathcal{N}$(0.42, 0.10) |
 
-where U(x, y) is a uniform distribution over [x, y]. 
+where $\mathcal{N}(\mu,\sigma)$ is a Gaussian distribution with mean $\mu$ and standard deviation $\sigma$.
 
 ## Acknowledging the code
 
 Please cite py-SP(k) using:
 
 ```
-@ARTICLE{spk,
-       author = {},
-        title = "{}",
-      journal = {\mnras},
-     keywords = {},
-         year = ,
-        month = ,
-       volume = {},
-       number = {},
-        pages = {},
-          doi = {},
-archivePrefix = {arXiv},
-       eprint = {},
- primaryClass = {astro-ph.CO},
-       adsurl = {},
-      adsnote = {}
+@ARTICLE{SPK_Salcido_2023,
+    author = {Salcido, Jaime and McCarthy, Ian G and Kwan, Juliana and Upadhye, Amol and Font, Andreea S},
+    title = "{SP(k) - A hydrodynamical simulation-based model for the impact of baryon physics on the non-linear matter power spectrum}",
+    journal = {Monthly Notices of the Royal Astronomical Society},
+    year = {2023},
+    month = {05},
+    issn = {0035-8711},
+    doi = {10.1093/mnras/stad1474},
+    url = {https://doi.org/10.1093/mnras/stad1474},
+    note = {stad1474},
+    eprint = {https://academic.oup.com/mnras/advance-article-pdf/doi/10.1093/mnras/stad1474/50356057/stad1474.pdf},
 }
 ```
 For any questions and enquires please contact me via email at *j.salcidonegrete@ljmu.ac.uk*
```

### Comparing `pyspk-1.2/README.md` & `pyspk-1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pyspk
+Version: 1.3
+Summary: Python package to predict the suppression of the total matter power spectrum due to baryonic physics
+Home-page: https://github.com/jemme07/pyspk
+Author: Jaime Salcido
+Author-email: j.salcidonegrete@ljmu.ac.uk
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # py-SP(k) - A hydrodynamical simulation-based model for the impact of baryon physics on the non-linear matter power spectrum
                           _____ ____   ____   _ 
         ____  __  __     / ___// __ \_/_/ /__| |
        / __ \/ / / /_____\__ \/ /_/ / // //_// /
       / /_/ / /_/ /_____/__/ / ____/ // ,<  / / 
      / .___/\__, /     /____/_/   / //_/|_|/_/  
     /_/    /____/                 |_|    /_/    
@@ -48,23 +61,23 @@
 fb_pivot = 10 ** 13.5
 
 k, sup = spk.sup_model(SO=200, z=z, fb_a=fb_a, fb_pow=fb_pow, fb_pivot=fb_pivot)
 ```
 
 ### Method 2: Redshift-dependent power-law fit to the $f_b$ - $M_\mathrm{halo}$ relation. 
 
-For the mass range that can be relatively well probed in current X-ray and Sunyaev-Zel'dovich effect observations (roughly $10^{13} \leq M_{500c} [\mathrm{M}_ \odot] \leq 10^{15}$), the total baryon fraction of haloes can be roughly approximated by a power-law with constant slope (e.g. Mulroy et al. 2019; Akino et al. 2022). Akino et al. 2022 determined the of the baryon budget for X-ray-selected galaxy groups and clusters using weak-lensing mass measurements. They provide a parametric redshift-dependent power-law fit to the gas mass - halo mass and stellar mass - halo mass relations, finding very little redshift evolution. 
+For the mass range that can be relatively well probed in current X-ray and Sunyaev-Zel'dovich effect observations (roughly $10^{13} \leq M_{500c} [\mathrm{M}_ \odot] \leq 10^{15}$), the total baryon fraction of haloes can be roughly approximated by a power-law with constant slope (e.g. Mulroy et al. 2019; Akino et al. 2022). Akino et al. (2022) determined the of the baryon budget for X-ray-selected galaxy groups and clusters using weak-lensing mass measurements. They provide a parametric redshift-dependent power-law fit to the gas mass - halo mass and stellar mass - halo mass relations, finding very little redshift evolution. 
 
-We implemented a modified version of the functional form presented in Akino et al. 2022, to fit the total $f_b$ - $M_\mathrm{halo}$ relation as follows:
+We implemented a modified version of the functional form presented in Akino et al. (2022), to fit the total $f_b$ - $M_\mathrm{halo}$ relation as follows:
 
 $$f_b/(\Omega_b/\Omega_m)= \left(\frac{0.1658}{\Omega_b/\Omega_m}\right) \left(\frac{e^\alpha}{100}\right) \left(\frac{M_{500c}}{10^{14} \mathrm{M}_ \odot}\right)^{\beta - 1} \left(\frac{E(z)}{E(0.3)}\right)^{\gamma},$$
 
 where $\alpha$ sets the power-law normalisation, $\beta$ sets power-law slope, $\gamma$ provides the redshift dependence and $E(z)$ is the usual dimensionless Hubble parameter. For simplicity, we use the cosmology implementation of `astropy` to specify the cosmological parameters in py-SP(k).
 
-Note that this power-law has a normalisation that is redshift dependent, while the the slop is constant in redshift. While this provides a less flexible approach compared with Methods 1 (simple power-law) and Method 3 (binned data), we find that this parametrisation agrees well with our simulations up to redshift $z=1$, which is the redshift range proved by Akino et al. 2022. For higher redshifts, we find that simulations require a mass-dependent slope, especially at the lower mass range required to predict the suppression of the total matter power spectrum at such redshifts. 
+Note that this power-law has a normalisation that is redshift dependent, while the the slope is constant in redshift. While this provides a less flexible approach compared with Methods 1 (simple power-law) and Method 3 (binned data), we find that this parametrisation provides a reasonable agreement with our simulations up to redshift $z=1$, which is the redshift range proved by Akino et al. (2022). For higher redshifts, we find that simulations require a mass-dependent slope, especially at the lower mass range required to predict the suppression of the total matter power spectrum at such redshifts. 
 
 In the following example we use the redshift-dependent power-law fit parameters with a flat LambdaCDM cosmology. Note that any `astropy` cosmology could be used instead.
 
 ```
 import pyspk.model as spk
 from astropy.cosmology import FlatLambdaCDM
 
@@ -80,70 +93,57 @@
 z = 0.5
 
 k, sup = spk.sup_model(SO=500, z=z, alpha=alpha, beta=beta, gamma=gamma, cosmo=cosmo)
 ```
 
 ### Method 3: Binned data for the $f_b$ - $M_\mathrm{halo}$ relation. 
 
-The final, and most flexible method is to provide py-SP(k) with the baryon fraction binned in bins of halo mass. This could be, for example, obtained from observational constraints, measured directly form simulations, or sampled from a predefined distribution or functional form. For an example using data obtained from the BAHAMAS simulations ([McCarthy et al. 2017](https://academic.oup.com/mnras/article/465/3/2936/2417021)), please refer to the [examples](https://github.com/jemme07/pyspk/blob/main/examples/pySPk_Examples.ipynb) provided. 
+The final, and most flexible method is to provide py-SP(k) with the baryon fraction binned in bins of halo mass. This could be, for example, obtained from observational constraints, measured directly form simulations, or sampled from a predefined distribution or functional form. For an example using data obtained from the BAHAMAS simulations (McCarthy et al. 2017), please refer to the [examples](https://github.com/jemme07/pyspk/blob/main/examples/pySPk_Examples.ipynb) provided. 
 
 
 ## Priors
 
-While py-SP(k) was calibrated using a wide range of sub-grid feedback parameters, some applications may require a more limited range of baryon fractions that encompass current observational constraints. For such applications, we used the gas mass - halo mass and stellar mass - halo mass constraints from Table 5 in Akino et al. 2022, and find the subset of simulations from our 400 models that agree with the inferred baryon budget at redshift $z=0.1$. We note that we constrained our simulations to within a normalisation of $\pm 3 \times \sigma$ at $M_{500c} = 10^{14} \mathrm{M}_ \odot$. 
-
-Using the simulations that fall within these constraints, we can impose observational priors for the redshift-dependent power-law fitting parameters for the $f_b$ - $M_\mathrm{halo}$ relation in Method 3 as follows:
-
-| Parameter   | Description        | Prior           |
-| ----------- | ------------------ | --------------- |
-| $\alpha$    | Normaliasation     | G(4.189, 0.066) |
-| $\beta$     | Slope              | G(1.273, 0.044) |
-| $\gamma$    | Redshift evolution | G(0.298, 0.063) |
+While py-SP(k) was calibrated using a wide range of sub-grid feedback parameters, some applications may require a more limited range of baryon fractions that encompass current observational constraints. For such applications, we used the gas mass - halo mass and stellar mass - halo mass constraints from the fits in Table 5 in Akino et al. (2022), and find the subset of simulations from our 400 models that agree to within $\pm 2$ or $3 \times \sigma$ of the inferred baryon budget at redshift $z=0.1$. We note that for our simulations, we include all stellar and gas particles within a spherical overdensity radius. Hence, in order to make reasonable comparisons with the fits in Akino et al. (2022), we included an additional 15\% contribution to the total stellar masses from the contribution of blue galaxies, and 30\% additional stellar mass to the brightest cluster galaxies (BCGs) to account for the diffuse intracluster light (ICL, see Akino et al. 2022). 
 
-where G(x, y) is a Gaussian distribution with center x and width y.
+We utilised the simulations satisfying these restrictions to determine the redshift-dependent power-law parameters for the $f_b$ - $M_\mathrm{halo}$ relation up to redshift $z=1$ (Method 2), and then utilised these parameters to infer suitable priors. We limited the fitting range to $6 \times 10^{12} \leq M_{500c} [\mathrm{M}_ \odot] \leq 10^{14}$. 
 
-A less conservative approach could be to use a flat priors over the entire range of parameters fitted to simulations that fall within Akino et al. 2022 these constraints:
+Priors inferred from simulations that fall within $\pm 2 \times \sigma$ of the inferred baryon budget:
 
 | Parameter   | Description        | Prior           |
 | ----------- | ------------------ | --------------- |
-| $\alpha$    | Normaliasation     | U(4.060, 4.306) |
-| $\beta$     | Slope              | U(1.199, 1.347) |
-| $\gamma$    | Redshift evolution | U(0.159, 0.414) |
+| $\alpha$    | Normaliasation     | $\mathcal{N}$(4.16, 0.07) |
+| $\beta$     | Slope              | $\mathcal{N}$(1.20, 0.05) |
+| $\gamma$    | Redshift evolution | $\mathcal{N}$(0.39, 0.09) |
 
-where U(x, y) is a uniform distribution over [x, y]. 
+where $\mathcal{N}(\mu,\sigma)$ is a Gaussian distribution with mean $\mu$ and standard deviation $\sigma$.
 
-Finally, the full range of fitted parameters spanned by our simulations, regardless of whether or not they agree with observational constraints is:
+Priors inferred from simulations that fall within $\pm 3 \times \sigma$ of the inferred baryon budget:
 
 | Parameter   | Description        | Prior           |
 | ----------- | ------------------ | --------------- |
-| $\alpha$    | Normaliasation     | U(3.060, 4.508) |
-| $\beta$     | Slope              | U(0.989, 1.620) |
-| $\gamma$    | Redshift evolution | U(0.046, 0.631) |
+| $\alpha$    | Normaliasation     | $\mathcal{N}$(4.18, 0.12) |
+| $\beta$     | Slope              | $\mathcal{N}$(1.26, 0.08) |
+| $\gamma$    | Redshift evolution | $\mathcal{N}$(0.42, 0.10) |
 
-where U(x, y) is a uniform distribution over [x, y]. 
+where $\mathcal{N}(\mu,\sigma)$ is a Gaussian distribution with mean $\mu$ and standard deviation $\sigma$.
 
 ## Acknowledging the code
 
 Please cite py-SP(k) using:
 
 ```
-@ARTICLE{spk,
-       author = {},
-        title = "{}",
-      journal = {\mnras},
-     keywords = {},
-         year = ,
-        month = ,
-       volume = {},
-       number = {},
-        pages = {},
-          doi = {},
-archivePrefix = {arXiv},
-       eprint = {},
- primaryClass = {astro-ph.CO},
-       adsurl = {},
-      adsnote = {}
+@ARTICLE{SPK_Salcido_2023,
+    author = {Salcido, Jaime and McCarthy, Ian G and Kwan, Juliana and Upadhye, Amol and Font, Andreea S},
+    title = "{SP(k) - A hydrodynamical simulation-based model for the impact of baryon physics on the non-linear matter power spectrum}",
+    journal = {Monthly Notices of the Royal Astronomical Society},
+    year = {2023},
+    month = {05},
+    issn = {0035-8711},
+    doi = {10.1093/mnras/stad1474},
+    url = {https://doi.org/10.1093/mnras/stad1474},
+    note = {stad1474},
+    eprint = {https://academic.oup.com/mnras/advance-article-pdf/doi/10.1093/mnras/stad1474/50356057/stad1474.pdf},
 }
 ```
 For any questions and enquires please contact me via email at *j.salcidonegrete@ljmu.ac.uk*
```

### Comparing `pyspk-1.2/pyspk/.DS_Store` & `pyspk-1.3/pyspk/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyspk-1.2/pyspk/__pycache__/fit_vals.cpython-39.pyc` & `pyspk-1.3/pyspk/__pycache__/fit_vals.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyspk-1.2/pyspk/__pycache__/model.cpython-39.pyc` & `pyspk-1.3/pyspk/__pycache__/model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyspk-1.2/pyspk/fit_vals.py` & `pyspk-1.3/pyspk/fit_vals.py`

 * *Files identical despite different names*

### Comparing `pyspk-1.2/pyspk/model.py` & `pyspk-1.3/pyspk/model.py`

 * *Files identical despite different names*

### Comparing `pyspk-1.2/pyspk/stat_errors_200.csv` & `pyspk-1.3/pyspk/stat_errors_200.csv`

 * *Files identical despite different names*

### Comparing `pyspk-1.2/pyspk/stat_errors_500.csv` & `pyspk-1.3/pyspk/stat_errors_500.csv`

 * *Files identical despite different names*

### Comparing `pyspk-1.2/pyspk.egg-info/PKG-INFO` & `pyspk-1.3/pyspk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspk
-Version: 1.2
+Version: 1.3
 Summary: Python package to predict the suppression of the total matter power spectrum due to baryonic physics
 Home-page: https://github.com/jemme07/pyspk
 Author: Jaime Salcido
 Author-email: j.salcidonegrete@ljmu.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
@@ -61,23 +61,23 @@
 fb_pivot = 10 ** 13.5
 
 k, sup = spk.sup_model(SO=200, z=z, fb_a=fb_a, fb_pow=fb_pow, fb_pivot=fb_pivot)
 ```
 
 ### Method 2: Redshift-dependent power-law fit to the $f_b$ - $M_\mathrm{halo}$ relation. 
 
-For the mass range that can be relatively well probed in current X-ray and Sunyaev-Zel'dovich effect observations (roughly $10^{13} \leq M_{500c} [\mathrm{M}_ \odot] \leq 10^{15}$), the total baryon fraction of haloes can be roughly approximated by a power-law with constant slope (e.g. Mulroy et al. 2019; Akino et al. 2022). Akino et al. 2022 determined the of the baryon budget for X-ray-selected galaxy groups and clusters using weak-lensing mass measurements. They provide a parametric redshift-dependent power-law fit to the gas mass - halo mass and stellar mass - halo mass relations, finding very little redshift evolution. 
+For the mass range that can be relatively well probed in current X-ray and Sunyaev-Zel'dovich effect observations (roughly $10^{13} \leq M_{500c} [\mathrm{M}_ \odot] \leq 10^{15}$), the total baryon fraction of haloes can be roughly approximated by a power-law with constant slope (e.g. Mulroy et al. 2019; Akino et al. 2022). Akino et al. (2022) determined the of the baryon budget for X-ray-selected galaxy groups and clusters using weak-lensing mass measurements. They provide a parametric redshift-dependent power-law fit to the gas mass - halo mass and stellar mass - halo mass relations, finding very little redshift evolution. 
 
-We implemented a modified version of the functional form presented in Akino et al. 2022, to fit the total $f_b$ - $M_\mathrm{halo}$ relation as follows:
+We implemented a modified version of the functional form presented in Akino et al. (2022), to fit the total $f_b$ - $M_\mathrm{halo}$ relation as follows:
 
 $$f_b/(\Omega_b/\Omega_m)= \left(\frac{0.1658}{\Omega_b/\Omega_m}\right) \left(\frac{e^\alpha}{100}\right) \left(\frac{M_{500c}}{10^{14} \mathrm{M}_ \odot}\right)^{\beta - 1} \left(\frac{E(z)}{E(0.3)}\right)^{\gamma},$$
 
 where $\alpha$ sets the power-law normalisation, $\beta$ sets power-law slope, $\gamma$ provides the redshift dependence and $E(z)$ is the usual dimensionless Hubble parameter. For simplicity, we use the cosmology implementation of `astropy` to specify the cosmological parameters in py-SP(k).
 
-Note that this power-law has a normalisation that is redshift dependent, while the the slop is constant in redshift. While this provides a less flexible approach compared with Methods 1 (simple power-law) and Method 3 (binned data), we find that this parametrisation agrees well with our simulations up to redshift $z=1$, which is the redshift range proved by Akino et al. 2022. For higher redshifts, we find that simulations require a mass-dependent slope, especially at the lower mass range required to predict the suppression of the total matter power spectrum at such redshifts. 
+Note that this power-law has a normalisation that is redshift dependent, while the the slope is constant in redshift. While this provides a less flexible approach compared with Methods 1 (simple power-law) and Method 3 (binned data), we find that this parametrisation provides a reasonable agreement with our simulations up to redshift $z=1$, which is the redshift range proved by Akino et al. (2022). For higher redshifts, we find that simulations require a mass-dependent slope, especially at the lower mass range required to predict the suppression of the total matter power spectrum at such redshifts. 
 
 In the following example we use the redshift-dependent power-law fit parameters with a flat LambdaCDM cosmology. Note that any `astropy` cosmology could be used instead.
 
 ```
 import pyspk.model as spk
 from astropy.cosmology import FlatLambdaCDM
 
@@ -93,70 +93,57 @@
 z = 0.5
 
 k, sup = spk.sup_model(SO=500, z=z, alpha=alpha, beta=beta, gamma=gamma, cosmo=cosmo)
 ```
 
 ### Method 3: Binned data for the $f_b$ - $M_\mathrm{halo}$ relation. 
 
-The final, and most flexible method is to provide py-SP(k) with the baryon fraction binned in bins of halo mass. This could be, for example, obtained from observational constraints, measured directly form simulations, or sampled from a predefined distribution or functional form. For an example using data obtained from the BAHAMAS simulations ([McCarthy et al. 2017](https://academic.oup.com/mnras/article/465/3/2936/2417021)), please refer to the [examples](https://github.com/jemme07/pyspk/blob/main/examples/pySPk_Examples.ipynb) provided. 
+The final, and most flexible method is to provide py-SP(k) with the baryon fraction binned in bins of halo mass. This could be, for example, obtained from observational constraints, measured directly form simulations, or sampled from a predefined distribution or functional form. For an example using data obtained from the BAHAMAS simulations (McCarthy et al. 2017), please refer to the [examples](https://github.com/jemme07/pyspk/blob/main/examples/pySPk_Examples.ipynb) provided. 
 
 
 ## Priors
 
-While py-SP(k) was calibrated using a wide range of sub-grid feedback parameters, some applications may require a more limited range of baryon fractions that encompass current observational constraints. For such applications, we used the gas mass - halo mass and stellar mass - halo mass constraints from Table 5 in Akino et al. 2022, and find the subset of simulations from our 400 models that agree with the inferred baryon budget at redshift $z=0.1$. We note that we constrained our simulations to within a normalisation of $\pm 3 \times \sigma$ at $M_{500c} = 10^{14} \mathrm{M}_ \odot$. 
+While py-SP(k) was calibrated using a wide range of sub-grid feedback parameters, some applications may require a more limited range of baryon fractions that encompass current observational constraints. For such applications, we used the gas mass - halo mass and stellar mass - halo mass constraints from the fits in Table 5 in Akino et al. (2022), and find the subset of simulations from our 400 models that agree to within $\pm 2$ or $3 \times \sigma$ of the inferred baryon budget at redshift $z=0.1$. We note that for our simulations, we include all stellar and gas particles within a spherical overdensity radius. Hence, in order to make reasonable comparisons with the fits in Akino et al. (2022), we included an additional 15\% contribution to the total stellar masses from the contribution of blue galaxies, and 30\% additional stellar mass to the brightest cluster galaxies (BCGs) to account for the diffuse intracluster light (ICL, see Akino et al. 2022). 
 
-Using the simulations that fall within these constraints, we can impose observational priors for the redshift-dependent power-law fitting parameters for the $f_b$ - $M_\mathrm{halo}$ relation in Method 3 as follows:
+We utilised the simulations satisfying these restrictions to determine the redshift-dependent power-law parameters for the $f_b$ - $M_\mathrm{halo}$ relation up to redshift $z=1$ (Method 2), and then utilised these parameters to infer suitable priors. We limited the fitting range to $6 \times 10^{12} \leq M_{500c} [\mathrm{M}_ \odot] \leq 10^{14}$. 
 
-| Parameter   | Description        | Prior           |
-| ----------- | ------------------ | --------------- |
-| $\alpha$    | Normaliasation     | G(4.189, 0.066) |
-| $\beta$     | Slope              | G(1.273, 0.044) |
-| $\gamma$    | Redshift evolution | G(0.298, 0.063) |
-
-where G(x, y) is a Gaussian distribution with center x and width y.
-
-A less conservative approach could be to use a flat priors over the entire range of parameters fitted to simulations that fall within Akino et al. 2022 these constraints:
+Priors inferred from simulations that fall within $\pm 2 \times \sigma$ of the inferred baryon budget:
 
 | Parameter   | Description        | Prior           |
 | ----------- | ------------------ | --------------- |
-| $\alpha$    | Normaliasation     | U(4.060, 4.306) |
-| $\beta$     | Slope              | U(1.199, 1.347) |
-| $\gamma$    | Redshift evolution | U(0.159, 0.414) |
+| $\alpha$    | Normaliasation     | $\mathcal{N}$(4.16, 0.07) |
+| $\beta$     | Slope              | $\mathcal{N}$(1.20, 0.05) |
+| $\gamma$    | Redshift evolution | $\mathcal{N}$(0.39, 0.09) |
 
-where U(x, y) is a uniform distribution over [x, y]. 
+where $\mathcal{N}(\mu,\sigma)$ is a Gaussian distribution with mean $\mu$ and standard deviation $\sigma$.
 
-Finally, the full range of fitted parameters spanned by our simulations, regardless of whether or not they agree with observational constraints is:
+Priors inferred from simulations that fall within $\pm 3 \times \sigma$ of the inferred baryon budget:
 
 | Parameter   | Description        | Prior           |
 | ----------- | ------------------ | --------------- |
-| $\alpha$    | Normaliasation     | U(3.060, 4.508) |
-| $\beta$     | Slope              | U(0.989, 1.620) |
-| $\gamma$    | Redshift evolution | U(0.046, 0.631) |
+| $\alpha$    | Normaliasation     | $\mathcal{N}$(4.18, 0.12) |
+| $\beta$     | Slope              | $\mathcal{N}$(1.26, 0.08) |
+| $\gamma$    | Redshift evolution | $\mathcal{N}$(0.42, 0.10) |
 
-where U(x, y) is a uniform distribution over [x, y]. 
+where $\mathcal{N}(\mu,\sigma)$ is a Gaussian distribution with mean $\mu$ and standard deviation $\sigma$.
 
 ## Acknowledging the code
 
 Please cite py-SP(k) using:
 
 ```
-@ARTICLE{spk,
-       author = {},
-        title = "{}",
-      journal = {\mnras},
-     keywords = {},
-         year = ,
-        month = ,
-       volume = {},
-       number = {},
-        pages = {},
-          doi = {},
-archivePrefix = {arXiv},
-       eprint = {},
- primaryClass = {astro-ph.CO},
-       adsurl = {},
-      adsnote = {}
+@ARTICLE{SPK_Salcido_2023,
+    author = {Salcido, Jaime and McCarthy, Ian G and Kwan, Juliana and Upadhye, Amol and Font, Andreea S},
+    title = "{SP(k) - A hydrodynamical simulation-based model for the impact of baryon physics on the non-linear matter power spectrum}",
+    journal = {Monthly Notices of the Royal Astronomical Society},
+    year = {2023},
+    month = {05},
+    issn = {0035-8711},
+    doi = {10.1093/mnras/stad1474},
+    url = {https://doi.org/10.1093/mnras/stad1474},
+    note = {stad1474},
+    eprint = {https://academic.oup.com/mnras/advance-article-pdf/doi/10.1093/mnras/stad1474/50356057/stad1474.pdf},
 }
 ```
 For any questions and enquires please contact me via email at *j.salcidonegrete@ljmu.ac.uk*
```

### Comparing `pyspk-1.2/setup.py` & `pyspk-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     print(long_description)
 
 setuptools.setup(
     name="pyspk",
-    version=1.2,
+    version=1.3,
     description="Python package to predict the suppression of the total matter power spectrum due to baryonic physics",
     url="https://github.com/jemme07/pyspk",
     author="Jaime Salcido",
     author_email="j.salcidonegrete@ljmu.ac.uk",
     packages=['pyspk'],
     long_description=long_description,
     long_description_content_type="text/markdown",
```

