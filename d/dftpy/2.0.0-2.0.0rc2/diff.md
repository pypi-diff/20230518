# Comparing `tmp/dftpy-2.0.0.tar.gz` & `tmp/dftpy-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dftpy-2.0.0.tar", last modified: Thu May 18 17:21:04 2023, max compression
+gzip compressed data, was "dftpy-2.0.0rc2.tar", last modified: Thu Oct 13 20:29:53 2022, max compression
```

## Comparing `dftpy-2.0.0.tar` & `dftpy-2.0.0rc2.tar`

### file list

```diff
@@ -1,276 +1,261 @@
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.062915 dftpy-2.0.0/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      126 2020-01-03 19:08:22.000000 dftpy-2.0.0/.gitattributes
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      175 2022-08-23 02:01:36.000000 dftpy-2.0.0/.gitignore
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1198 2021-02-06 01:38:39.000000 dftpy-2.0.0/.gitlab-ci.yml
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1097 2020-01-03 19:08:22.000000 dftpy-2.0.0/LICENSE.txt
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      149 2023-02-21 20:09:34.000000 dftpy-2.0.0/MANIFEST.in
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      954 2023-05-18 17:21:04.062915 dftpy-2.0.0/PKG-INFO
--rw-rw-r--   0 sxc       (1000) sxc       (1000)       95 2022-08-23 02:01:36.000000 dftpy-2.0.0/README.md
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.038916 dftpy-2.0.0/doc/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1036 2022-08-23 02:01:36.000000 dftpy-2.0.0/doc/Makefile
--rwxrwxr-x   0 sxc       (1000) sxc       (1000)     4189 2022-06-06 15:29:01.000000 dftpy-2.0.0/doc/gen_doc.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      795 2020-01-03 19:08:22.000000 dftpy-2.0.0/doc/make.bat
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.038916 dftpy-2.0.0/doc/source/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1344 2022-08-23 02:01:36.000000 dftpy-2.0.0/doc/source/conf.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      957 2022-08-23 02:01:36.000000 dftpy-2.0.0/doc/source/contact.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      557 2022-08-23 02:01:36.000000 dftpy-2.0.0/doc/source/faq.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      637 2022-08-23 02:01:36.000000 dftpy-2.0.0/doc/source/index.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1745 2023-05-18 17:13:10.000000 dftpy-2.0.0/doc/source/install.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     5597 2022-08-23 02:01:36.000000 dftpy-2.0.0/doc/source/ofdft.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1364 2023-05-18 17:13:10.000000 dftpy-2.0.0/doc/source/releases.rst
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.038916 dftpy-2.0.0/doc/source/static/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      436 2022-08-23 02:01:36.000000 dftpy-2.0.0/doc/source/static/custom.css
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   270398 2022-08-23 02:01:36.000000 dftpy-2.0.0/doc/source/static/dftpy.ico
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    27665 2022-08-23 02:01:36.000000 dftpy-2.0.0/doc/source/static/dftpy.jpg
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     7269 2022-08-23 02:01:36.000000 dftpy-2.0.0/doc/source/static/dftpy.png
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   254932 2022-08-23 02:01:36.000000 dftpy-2.0.0/doc/source/static/dftpy_new_bkg.png
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.038916 dftpy-2.0.0/doc/source/templates/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      600 2022-08-23 02:01:36.000000 dftpy-2.0.0/doc/source/templates/breadcrumbs.html
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      593 2022-08-23 02:01:36.000000 dftpy-2.0.0/doc/source/templates/footer.html
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.038916 dftpy-2.0.0/doc/source/tutorials/
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.038916 dftpy-2.0.0/doc/source/tutorials/jupyter/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    23595 2020-01-09 02:43:27.000000 dftpy-2.0.0/doc/source/tutorials/jupyter/density.png
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   220165 2023-05-18 17:13:10.000000 dftpy-2.0.0/doc/source/tutorials/jupyter/density_optimization.ipynb
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    19646 2020-01-09 02:43:27.000000 dftpy-2.0.0/doc/source/tutorials/jupyter/ions.png
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   747735 2021-12-15 03:11:30.000000 dftpy-2.0.0/doc/source/tutorials/jupyter/movie.gif
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   393516 2023-05-18 17:13:10.000000 dftpy-2.0.0/doc/source/tutorials/jupyter/td-ofdft-tutorial.ipynb
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.038916 dftpy-2.0.0/doc/source/tutorials/ofdft/
--rwxrwxr-x   0 sxc       (1000) sxc       (1000)      182 2020-01-03 19:08:22.000000 dftpy-2.0.0/doc/source/tutorials/ofdft/ase_traj.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      382 2020-01-09 02:43:27.000000 dftpy-2.0.0/doc/source/tutorials/ofdft/md.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1790 2021-12-15 03:11:30.000000 dftpy-2.0.0/doc/source/tutorials/ofdft/nvt.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      432 2022-08-23 02:01:36.000000 dftpy-2.0.0/doc/source/tutorials/ofdft/optimize.rst
--rwxrwxr-x   0 sxc       (1000) sxc       (1000)     1301 2020-01-03 19:08:22.000000 dftpy-2.0.0/doc/source/tutorials/ofdft/relax.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      711 2021-06-10 20:50:12.000000 dftpy-2.0.0/doc/source/tutorials/ofdft/relax.rst
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.038916 dftpy-2.0.0/doc/source/tutorials/tddft/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      437 2020-01-08 20:50:55.000000 dftpy-2.0.0/doc/source/tutorials/tddft/optimize.ini
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      516 2020-01-08 20:50:55.000000 dftpy-2.0.0/doc/source/tutorials/tddft/propagate.ini
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1229 2021-12-15 03:11:30.000000 dftpy-2.0.0/doc/source/tutorials/tddft/propagate.rst
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      453 2022-08-23 02:01:36.000000 dftpy-2.0.0/doc/source/tutorials/tutorials.rst
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.034916 dftpy-2.0.0/examples/
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.050915 dftpy-2.0.0/examples/DATA/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)  1605583 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/Al_fde_rho.pp
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   196436 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/Al_lda.oe01.recpot
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   196502 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/As_lda.oe04.recpot
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2960 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/GaAs.cif
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      686 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/GaAs.vasp
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      411 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/GaAs.xyz
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1001 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/GaAs_random.vasp
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   208643 2020-01-09 21:41:19.000000 dftpy-2.0.0/examples/DATA/GaAs_random.xsf
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   196489 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/Ga_lda.oe04.recpot
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      839 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/DATA/Mg8.vasp
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    98081 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/DATA/Mg_OEPP_PZ.UPF
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      655 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/Mg_cluster.vasp
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   196232 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/Mg_lda.oe01.recpot
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   233666 2021-12-15 03:08:34.000000 dftpy-2.0.0/examples/DATA/al.gga.recpot
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    69674 2022-06-06 15:29:01.000000 dftpy-2.0.0/examples/DATA/al.lda.lps
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    69674 2022-06-06 15:29:01.000000 dftpy-2.0.0/examples/DATA/al.lda.psp
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   492756 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/al.lda.recpot
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   224896 2022-06-06 15:29:01.000000 dftpy-2.0.0/examples/DATA/al.lda.upf
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      831 2023-01-24 18:47:21.000000 dftpy-2.0.0/examples/DATA/al_random.in
--rw-rw-r--   0 sxc       (1000) sxc       (1000)  3705904 2023-01-24 18:47:21.000000 dftpy-2.0.0/examples/DATA/al_random.xsf
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   101843 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/as.lda.recpot
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      949 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/ase_opt.traj
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      735 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/cd.vasp
--rw-rw-r--   0 sxc       (1000) sxc       (1000)       81 2023-01-14 15:28:31.000000 dftpy-2.0.0/examples/DATA/fcc.vasp
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    67650 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/ga.lda.recpot
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      491 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/hd.vasp
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   507599 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/in.lda.recpot
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     6437 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/initial_atoms_md.traj
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   233593 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/li.lda.recpot
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    25874 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/md.traj
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   492424 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/mg.lda.recpot
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   337875 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/p.lda.recpot
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   338504 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/sb.lda.recpot
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   233695 2021-12-15 03:08:34.000000 dftpy-2.0.0/examples/DATA/si.gga.recpot
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    95514 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/DATA/si.lda.recpot
--rw-rw-r--   0 sxc       (1000) sxc       (1000)  1280986 2023-05-03 20:24:26.000000 dftpy-2.0.0/examples/DATA/ti.xsf
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   577420 2023-05-03 20:24:26.000000 dftpy-2.0.0/examples/DATA/ti_pbe_v1.4.uspp.F.UPF
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.050915 dftpy-2.0.0/examples/md/
--rwxrwxr-x   0 sxc       (1000) sxc       (1000)     2463 2023-05-03 20:24:26.000000 dftpy-2.0.0/examples/md/test_ase_npt.py
--rwxrwxr-x   0 sxc       (1000) sxc       (1000)     2156 2023-05-03 20:24:26.000000 dftpy-2.0.0/examples/md/test_ase_nvt.py
--rwxrwxr-x   0 sxc       (1000) sxc       (1000)     2346 2023-05-03 20:24:26.000000 dftpy-2.0.0/examples/md/test_ase_nvt_nh.py
--rwxrwxr-x   0 sxc       (1000) sxc       (1000)      197 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/md/traj2xyz.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.050915 dftpy-2.0.0/examples/notebooks/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   220165 2023-05-18 17:13:10.000000 dftpy-2.0.0/examples/notebooks/density_optimization.ipynb
--rw-rw-r--   0 sxc       (1000) sxc       (1000)   393516 2023-05-18 17:13:10.000000 dftpy-2.0.0/examples/notebooks/td-ofdft-tutorial.ipynb
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.050915 dftpy-2.0.0/examples/ofdft/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      742 2021-12-15 03:08:34.000000 dftpy-2.0.0/examples/ofdft/config.ini
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      619 2020-01-03 19:08:22.000000 dftpy-2.0.0/examples/ofdft/isolate.ini
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      342 2023-05-18 17:07:12.000000 dftpy-2.0.0/examples/ofdft/optim.ini
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2297 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/ofdft/optim.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      342 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/ofdft/optim_pbe.ini
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1159 2022-08-26 14:23:30.000000 dftpy-2.0.0/examples/ofdft/simple.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.050915 dftpy-2.0.0/examples/relax/
--rwxrwxr-x   0 sxc       (1000) sxc       (1000)     1916 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/relax/test_ase_opt.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.054915 dftpy-2.0.0/examples/td-ofdft/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      450 2021-12-15 03:11:30.000000 dftpy-2.0.0/examples/td-ofdft/casida.ini
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      442 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/td-ofdft/optimize.ini
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      419 2021-12-15 03:11:30.000000 dftpy-2.0.0/examples/td-ofdft/propagate-restart.ini
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      407 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/td-ofdft/propagate.ini
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.054915 dftpy-2.0.0/examples/test/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      297 2020-01-09 02:43:44.000000 dftpy-2.0.0/examples/test/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     3969 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/test/common.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1554 2023-05-03 20:24:26.000000 dftpy-2.0.0/examples/test/test_ase_md.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1459 2023-05-03 20:24:26.000000 dftpy-2.0.0/examples/test/test_ase_opt.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      952 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/test/test_ase_pmg_io.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2052 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/test/test_density_opt.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2354 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/test/test_ewald.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     3842 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/test/test_field.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1628 2023-01-20 03:18:33.000000 dftpy-2.0.0/examples/test/test_functional.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1210 2023-05-03 20:24:26.000000 dftpy-2.0.0/examples/test/test_functional_LibXC.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1253 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/test/test_grid.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1102 2021-12-15 03:11:30.000000 dftpy-2.0.0/examples/test/test_linear_solver.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      852 2021-12-15 03:11:30.000000 dftpy-2.0.0/examples/test/test_mpi_grid.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2313 2023-05-03 20:24:26.000000 dftpy-2.0.0/examples/test/test_pme.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2929 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/test/test_propagator.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1091 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/test/test_read_pp.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1034 2023-01-24 18:47:21.000000 dftpy-2.0.0/examples/test/test_rvv10.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2102 2022-08-23 02:01:36.000000 dftpy-2.0.0/examples/test/test_snpy.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1626 2023-05-03 20:24:26.000000 dftpy-2.0.0/examples/test/test_xc.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      104 2023-05-18 16:42:22.000000 dftpy-2.0.0/requirements.txt
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.054915 dftpy-2.0.0/scripts/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2888 2021-12-15 03:11:30.000000 dftpy-2.0.0/scripts/convertPP.py
--rwxrwxr-x   0 sxc       (1000) sxc       (1000)     1499 2022-08-23 02:01:36.000000 dftpy-2.0.0/scripts/convert_den.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1485 2022-08-23 02:01:36.000000 dftpy-2.0.0/scripts/convert_td.py
--rwxrwxr-x   0 sxc       (1000) sxc       (1000)      217 2021-12-15 03:11:30.000000 dftpy-2.0.0/scripts/dftpy
--rwxrwxr-x   0 sxc       (1000) sxc       (1000)     1161 2021-12-15 03:08:34.000000 dftpy-2.0.0/scripts/invert
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     5864 2023-01-10 15:16:28.000000 dftpy-2.0.0/scripts/opt_layer_pseudo.py
--rwxrwxr-x   0 sxc       (1000) sxc       (1000)     8906 2023-01-10 15:16:28.000000 dftpy-2.0.0/scripts/quadrupole.py
--rwxrwxr-x   0 sxc       (1000) sxc       (1000)     2121 2023-01-10 15:16:28.000000 dftpy-2.0.0/scripts/rtc_runner
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     5928 2023-01-10 15:16:28.000000 dftpy-2.0.0/scripts/test_layer_pseudo.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)       79 2023-05-18 17:21:04.062915 dftpy-2.0.0/setup.cfg
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2652 2023-05-18 17:20:56.000000 dftpy-2.0.0/setup.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.034916 dftpy-2.0.0/src/
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.054915 dftpy-2.0.0/src/dftpy/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      481 2023-05-18 17:16:44.000000 dftpy-2.0.0/src/dftpy/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)       39 2021-12-15 20:59:24.000000 dftpy-2.0.0/src/dftpy/__main__.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.054915 dftpy-2.0.0/src/dftpy/api/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)        0 2021-12-15 20:59:24.000000 dftpy-2.0.0/src/dftpy/api/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     3352 2023-02-28 14:21:18.000000 dftpy-2.0.0/src/dftpy/api/api4ase.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     3658 2022-06-06 15:29:01.000000 dftpy-2.0.0/src/dftpy/api/dftd4.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.058915 dftpy-2.0.0/src/dftpy/config/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)       69 2021-12-15 20:59:24.000000 dftpy-2.0.0/src/dftpy/config/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     4609 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/config/config.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     5202 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/config/config_entry.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    22102 2023-04-13 19:26:47.000000 dftpy-2.0.0/src/dftpy/config/configentries.json
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2697 2022-08-26 15:18:11.000000 dftpy-2.0.0/src/dftpy/constants.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.058915 dftpy-2.0.0/src/dftpy/cui/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)        0 2021-12-15 20:59:24.000000 dftpy-2.0.0/src/dftpy/cui/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2648 2023-02-28 14:21:18.000000 dftpy-2.0.0/src/dftpy/cui/main.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.058915 dftpy-2.0.0/src/dftpy/density/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)       76 2023-02-28 14:21:18.000000 dftpy-2.0.0/src/dftpy/density/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    11216 2023-05-03 20:24:26.000000 dftpy-2.0.0/src/dftpy/density/density.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    36414 2023-05-03 20:24:26.000000 dftpy-2.0.0/src/dftpy/ewald.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2704 2021-12-15 20:59:24.000000 dftpy-2.0.0/src/dftpy/fft.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    29351 2023-02-24 21:22:54.000000 dftpy-2.0.0/src/dftpy/field.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.058915 dftpy-2.0.0/src/dftpy/formats/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)        0 2022-06-10 13:11:08.000000 dftpy-2.0.0/src/dftpy/formats/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1515 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/formats/ase_io.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     3487 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/formats/cube.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1333 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/formats/den.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     8181 2023-01-24 18:47:21.000000 dftpy-2.0.0/src/dftpy/formats/io.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     5885 2022-06-06 15:29:01.000000 dftpy-2.0.0/src/dftpy/formats/npy.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      977 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/formats/pmg_io.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     7820 2023-01-24 18:47:21.000000 dftpy-2.0.0/src/dftpy/formats/qepp.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     4870 2023-04-10 15:36:18.000000 dftpy-2.0.0/src/dftpy/formats/snpy.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2566 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/formats/vasp.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     9597 2023-05-03 20:24:26.000000 dftpy-2.0.0/src/dftpy/formats/xsf.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1637 2023-01-10 15:16:28.000000 dftpy-2.0.0/src/dftpy/formats/xyz.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.058915 dftpy-2.0.0/src/dftpy/functional/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1397 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/functional/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1624 2023-01-24 18:47:21.000000 dftpy-2.0.0/src/dftpy/functional/abstract_functional.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      894 2023-02-28 14:21:18.000000 dftpy-2.0.0/src/dftpy/functional/external_potential.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     3591 2023-02-28 14:21:18.000000 dftpy-2.0.0/src/dftpy/functional/functional_output.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2666 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/functional/hartree.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.058915 dftpy-2.0.0/src/dftpy/functional/kedf/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    17102 2023-05-18 13:43:26.000000 dftpy-2.0.0/src/dftpy/functional/kedf/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     7191 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/functional/kedf/fp.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    48091 2023-05-08 18:56:14.000000 dftpy-2.0.0/src/dftpy/functional/kedf/gga.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    16248 2023-02-28 14:21:18.000000 dftpy-2.0.0/src/dftpy/functional/kedf/hc.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    16487 2023-05-18 13:43:26.000000 dftpy-2.0.0/src/dftpy/functional/kedf/kernel.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2197 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/functional/kedf/lkt.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    20136 2023-01-10 15:16:28.000000 dftpy-2.0.0/src/dftpy/functional/kedf/lwt.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     3852 2023-05-18 13:43:26.000000 dftpy-2.0.0/src/dftpy/functional/kedf/mgp.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     3668 2023-05-15 22:33:28.000000 dftpy-2.0.0/src/dftpy/functional/kedf/sm.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     5712 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/functional/kedf/tf.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     4933 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/functional/kedf/vw.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     5151 2023-05-03 20:23:01.000000 dftpy-2.0.0/src/dftpy/functional/kedf/wt.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.058915 dftpy-2.0.0/src/dftpy/functional/nonadiabatic/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1149 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/functional/nonadiabatic/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2419 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/functional/nonadiabatic/jp.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1267 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/functional/nonadiabatic/wcdhc.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.058915 dftpy-2.0.0/src/dftpy/functional/pseudo/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    28607 2023-05-09 17:59:26.000000 dftpy-2.0.0/src/dftpy/functional/pseudo/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2197 2022-06-06 15:29:01.000000 dftpy-2.0.0/src/dftpy/functional/pseudo/abstract_pseudo.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2563 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/functional/pseudo/layer_pseudo.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2462 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/functional/pseudo/psp.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1559 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/functional/pseudo/recpot.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     7315 2023-05-03 20:24:26.000000 dftpy-2.0.0/src/dftpy/functional/pseudo/upf.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     3373 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/functional/pseudo/usp.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     3025 2022-06-06 15:29:01.000000 dftpy-2.0.0/src/dftpy/functional/pseudo/xml.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)       34 2023-01-24 18:47:21.000000 dftpy-2.0.0/src/dftpy/functional/semilocal_xc.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     7100 2023-05-18 16:32:19.000000 dftpy-2.0.0/src/dftpy/functional/total_functional.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.058915 dftpy-2.0.0/src/dftpy/functional/xc/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2761 2023-05-03 20:24:26.000000 dftpy-2.0.0/src/dftpy/functional/xc/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     9520 2023-04-07 01:43:53.000000 dftpy-2.0.0/src/dftpy/functional/xc/rvv10.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    20079 2023-05-03 20:24:26.000000 dftpy-2.0.0/src/dftpy/functional/xc/semilocal_xc.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     8582 2023-01-24 18:47:21.000000 dftpy-2.0.0/src/dftpy/functional/xc/xc.json
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    27071 2023-05-03 20:24:26.000000 dftpy-2.0.0/src/dftpy/grid.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    13165 2023-05-03 20:24:26.000000 dftpy-2.0.0/src/dftpy/interface.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.058915 dftpy-2.0.0/src/dftpy/invert/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1941 2023-04-10 15:36:18.000000 dftpy-2.0.0/src/dftpy/invert/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      223 2023-04-10 15:36:18.000000 dftpy-2.0.0/src/dftpy/invert/analysis.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1168 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/inverter.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     4790 2023-01-24 18:47:21.000000 dftpy-2.0.0/src/dftpy/ions.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2785 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/linear_solver.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    15721 2023-05-03 20:24:26.000000 dftpy-2.0.0/src/dftpy/math_utils.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.062915 dftpy-2.0.0/src/dftpy/mixer/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1556 2023-02-28 14:21:18.000000 dftpy-2.0.0/src/dftpy/mixer/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1076 2023-02-28 14:21:18.000000 dftpy-2.0.0/src/dftpy/mixer/linear.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     5538 2023-02-28 14:21:18.000000 dftpy-2.0.0/src/dftpy/mixer/mixer.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     4806 2023-02-28 14:21:18.000000 dftpy-2.0.0/src/dftpy/mixer/pulay.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.062915 dftpy-2.0.0/src/dftpy/mpi/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      248 2022-06-06 15:29:01.000000 dftpy-2.0.0/src/dftpy/mpi/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2961 2023-01-24 18:47:21.000000 dftpy-2.0.0/src/dftpy/mpi/mp_mpi4py.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2614 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/mpi/mp_serial.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    10314 2023-01-20 20:00:38.000000 dftpy-2.0.0/src/dftpy/mpi/mpi.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1202 2022-06-06 15:29:01.000000 dftpy-2.0.0/src/dftpy/mpi/utils.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.062915 dftpy-2.0.0/src/dftpy/optimization/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)       84 2023-02-28 14:21:18.000000 dftpy-2.0.0/src/dftpy/optimization/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    21103 2023-02-28 14:21:18.000000 dftpy-2.0.0/src/dftpy/optimization/optimization.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     4001 2023-02-28 14:21:18.000000 dftpy-2.0.0/src/dftpy/optimization/scf.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    10612 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/optimize.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.062915 dftpy-2.0.0/src/dftpy/properties/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)       71 2021-12-15 20:59:24.000000 dftpy-2.0.0/src/dftpy/properties/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      251 2021-12-15 20:59:24.000000 dftpy-2.0.0/src/dftpy/properties/potential.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.062915 dftpy-2.0.0/src/dftpy/td/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)        0 2021-12-15 20:59:24.000000 dftpy-2.0.0/src/dftpy/td/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     8385 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/td/casida.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     6571 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/td/hamiltonian.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2661 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/td/interface.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1934 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/td/operator.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     5104 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/td/predictor_corrector.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.062915 dftpy-2.0.0/src/dftpy/td/propagator/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1092 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/td/propagator/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1748 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/td/propagator/abstract_propagator.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     6806 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/td/propagator/crank_nicholson.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2017 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/td/propagator/taylor.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)    13333 2023-01-10 15:16:28.000000 dftpy-2.0.0/src/dftpy/td/real_time_runner.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1215 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/td/utils.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     3458 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/time_data.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.062915 dftpy-2.0.0/src/dftpy/utils/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1703 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/utils/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     9932 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/utils/utils.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.062915 dftpy-2.0.0/src/dftpy/visualize/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      991 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/visualize/__init__.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      217 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/visualize/ase_viewer.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      822 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/visualize/ipv_viewer.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     1099 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/visualize/jupyter.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     2778 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/visualize/mpl_viewer.py
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      868 2022-08-23 02:01:36.000000 dftpy-2.0.0/src/dftpy/visualize/vesta_viewer.py
-drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2023-05-18 17:21:04.054915 dftpy-2.0.0/src/dftpy.egg-info/
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      954 2023-05-18 17:21:03.000000 dftpy-2.0.0/src/dftpy.egg-info/PKG-INFO
--rw-rw-r--   0 sxc       (1000) sxc       (1000)     6845 2023-05-18 17:21:04.000000 dftpy-2.0.0/src/dftpy.egg-info/SOURCES.txt
--rw-rw-r--   0 sxc       (1000) sxc       (1000)        1 2023-05-18 17:21:03.000000 dftpy-2.0.0/src/dftpy.egg-info/dependency_links.txt
--rw-rw-r--   0 sxc       (1000) sxc       (1000)      289 2023-05-18 17:21:03.000000 dftpy-2.0.0/src/dftpy.egg-info/requires.txt
--rw-rw-r--   0 sxc       (1000) sxc       (1000)        6 2023-05-18 17:21:03.000000 dftpy-2.0.0/src/dftpy.egg-info/top_level.txt
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.401878 dftpy-2.0.0rc2/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      126 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/.gitattributes
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      175 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/.gitignore
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1198 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/.gitlab-ci.yml
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1097 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/LICENSE.txt
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      124 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/MANIFEST.in
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      982 2022-10-13 20:29:53.401878 dftpy-2.0.0rc2/PKG-INFO
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)       95 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/README.md
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.377879 dftpy-2.0.0rc2/doc/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1036 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/Makefile
+-rwxrwxr-x   0 sxc       (1000) sxc       (1000)     4189 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/gen_doc.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      795 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/make.bat
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.377879 dftpy-2.0.0rc2/doc/source/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1344 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/conf.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      957 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/contact.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      557 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/faq.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      637 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/index.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1702 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/install.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     5597 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/ofdft.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1339 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/releases.rst
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.377879 dftpy-2.0.0rc2/doc/source/static/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      436 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/static/custom.css
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   270398 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/static/dftpy.ico
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    27665 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/static/dftpy.jpg
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     7269 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/static/dftpy.png
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   254932 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/static/dftpy_new_bkg.png
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.377879 dftpy-2.0.0rc2/doc/source/templates/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      600 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/templates/breadcrumbs.html
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      593 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/templates/footer.html
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.377879 dftpy-2.0.0rc2/doc/source/tutorials/
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.381879 dftpy-2.0.0rc2/doc/source/tutorials/jupyter/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    23595 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/tutorials/jupyter/density.png
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   297732 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/tutorials/jupyter/density_optimization.ipynb
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    19646 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/tutorials/jupyter/ions.png
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   747735 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/tutorials/jupyter/movie.gif
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   136661 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/tutorials/jupyter/td-ofdft-tutorial.ipynb
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.381879 dftpy-2.0.0rc2/doc/source/tutorials/ofdft/
+-rwxrwxr-x   0 sxc       (1000) sxc       (1000)      182 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/tutorials/ofdft/ase_traj.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      382 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/tutorials/ofdft/md.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1790 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/tutorials/ofdft/nvt.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      432 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/tutorials/ofdft/optimize.rst
+-rwxrwxr-x   0 sxc       (1000) sxc       (1000)     1301 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/tutorials/ofdft/relax.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      711 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/tutorials/ofdft/relax.rst
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.381879 dftpy-2.0.0rc2/doc/source/tutorials/tddft/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      437 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/tutorials/tddft/optimize.ini
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      516 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/tutorials/tddft/propagate.ini
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1229 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/tutorials/tddft/propagate.rst
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      453 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/doc/source/tutorials/tutorials.rst
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.377879 dftpy-2.0.0rc2/examples/
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.389879 dftpy-2.0.0rc2/examples/DATA/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)  1605583 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/Al_fde_rho.pp
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   196436 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/Al_lda.oe01.recpot
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   196502 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/As_lda.oe04.recpot
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2960 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/GaAs.cif
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      686 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/GaAs.vasp
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      411 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/GaAs.xyz
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1001 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/GaAs_random.vasp
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   208643 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/GaAs_random.xsf
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   196489 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/Ga_lda.oe04.recpot
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      839 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/Mg8.vasp
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    98081 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/Mg_OEPP_PZ.UPF
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      655 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/Mg_cluster.vasp
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   196232 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/Mg_lda.oe01.recpot
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   233666 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/al.gga.recpot
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    69674 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/al.lda.lps
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    69674 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/al.lda.psp
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   492756 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/al.lda.recpot
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   224896 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/al.lda.upf
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   101843 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/as.lda.recpot
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      949 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/ase_opt.traj
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      735 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/cd.vasp
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)       81 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/fcc.vasp
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    67650 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/ga.lda.recpot
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      491 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/hd.vasp
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   507599 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/in.lda.recpot
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     6437 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/initial_atoms_md.traj
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   233593 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/li.lda.recpot
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    25874 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/md.traj
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   492424 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/mg.lda.recpot
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   337875 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/p.lda.recpot
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   338504 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/sb.lda.recpot
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   233695 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/si.gga.recpot
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    95514 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/DATA/si.lda.recpot
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.389879 dftpy-2.0.0rc2/examples/md/
+-rwxrwxr-x   0 sxc       (1000) sxc       (1000)     2472 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/md/test_ase_npt.py
+-rwxrwxr-x   0 sxc       (1000) sxc       (1000)     2166 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/md/test_ase_nvt.py
+-rwxrwxr-x   0 sxc       (1000) sxc       (1000)     2356 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/md/test_ase_nvt_nh.py
+-rwxrwxr-x   0 sxc       (1000) sxc       (1000)      197 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/md/traj2xyz.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.389879 dftpy-2.0.0rc2/examples/notebooks/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   297732 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/notebooks/density_optimization.ipynb
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)   136661 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/notebooks/td-ofdft-tutorial.ipynb
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.389879 dftpy-2.0.0rc2/examples/ofdft/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      742 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/ofdft/config.ini
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      619 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/ofdft/isolate.ini
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      342 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/ofdft/optim.ini
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2297 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/ofdft/optim.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      342 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/ofdft/optim_pbe.ini
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1159 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/ofdft/simple.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.389879 dftpy-2.0.0rc2/examples/relax/
+-rwxrwxr-x   0 sxc       (1000) sxc       (1000)     1916 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/relax/test_ase_opt.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.389879 dftpy-2.0.0rc2/examples/td-ofdft/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      450 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/td-ofdft/casida.ini
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      442 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/td-ofdft/optimize.ini
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      419 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/td-ofdft/propagate-restart.ini
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      407 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/td-ofdft/propagate.ini
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.389879 dftpy-2.0.0rc2/examples/test/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      297 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     3969 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/common.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1725 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/test_ase_md.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1636 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/test_ase_opt.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      952 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/test_ase_pmg_io.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2052 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/test_density_opt.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2354 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/test_ewald.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     3842 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/test_field.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1628 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/test_functional.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1350 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/test_functional_LibXC.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1253 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/test_grid.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1102 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/test_linear_solver.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      852 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/test_mpi_grid.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2311 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/test_pme.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2929 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/test_propagator.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1091 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/test_read_pp.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2102 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/examples/test/test_snpy.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)       86 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/requirements.txt
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.393879 dftpy-2.0.0rc2/scripts/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2888 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/scripts/convertPP.py
+-rwxrwxr-x   0 sxc       (1000) sxc       (1000)     1499 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/scripts/convert_den.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1485 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/scripts/convert_td.py
+-rwxrwxr-x   0 sxc       (1000) sxc       (1000)      217 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/scripts/dftpy
+-rwxrwxr-x   0 sxc       (1000) sxc       (1000)     1161 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/scripts/invert
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     5864 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/scripts/opt_layer_pseudo.py
+-rwxrwxr-x   0 sxc       (1000) sxc       (1000)     8906 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/scripts/quadrupole.py
+-rwxrwxr-x   0 sxc       (1000) sxc       (1000)     2121 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/scripts/rtc_runner
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     5928 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/scripts/test_layer_pseudo.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)       79 2022-10-13 20:29:53.401878 dftpy-2.0.0rc2/setup.cfg
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2470 2022-10-13 20:24:38.000000 dftpy-2.0.0rc2/setup.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.377879 dftpy-2.0.0rc2/src/
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.393879 dftpy-2.0.0rc2/src/dftpy/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      484 2022-10-13 20:28:26.000000 dftpy-2.0.0rc2/src/dftpy/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)       39 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/__main__.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.393879 dftpy-2.0.0rc2/src/dftpy/api/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)        0 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/api/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     3546 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/api/api4ase.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     3658 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/api/dftd4.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.393879 dftpy-2.0.0rc2/src/dftpy/config/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)       69 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/config/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     4609 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/config/config.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     5202 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/config/config_entry.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    21854 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/config/configentries.json
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2697 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/constants.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.393879 dftpy-2.0.0rc2/src/dftpy/cui/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)        0 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/cui/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2703 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/cui/main.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.393879 dftpy-2.0.0rc2/src/dftpy/density/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    16383 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/density/density.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    36662 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/ewald.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2704 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/fft.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    28424 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/field.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.393879 dftpy-2.0.0rc2/src/dftpy/formats/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)        0 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/formats/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1515 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/formats/ase_io.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     3487 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/formats/cube.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1333 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/formats/den.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     6933 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/formats/io.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     5885 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/formats/npy.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      977 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/formats/pmg_io.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     7809 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/formats/qepp.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     4900 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/formats/snpy.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2566 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/formats/vasp.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     9530 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/formats/xsf.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1639 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/formats/xyz.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.397879 dftpy-2.0.0rc2/src/dftpy/functional/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1397 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1503 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/abstract_functional.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      846 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/external_potential.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     3538 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/functional_output.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2666 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/hartree.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.397879 dftpy-2.0.0rc2/src/dftpy/functional/kedf/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    16547 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/kedf/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     7191 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/kedf/fp.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    45297 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/kedf/gga.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    16257 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/kedf/hc.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    16557 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/kedf/kernel.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2197 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/kedf/lkt.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    20136 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/kedf/lwt.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     3489 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/kedf/mgp.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     3668 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/kedf/sm.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     5712 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/kedf/tf.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     4933 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/kedf/vw.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     5151 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/kedf/wt.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.397879 dftpy-2.0.0rc2/src/dftpy/functional/nonadiabatic/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1149 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/nonadiabatic/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2419 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/nonadiabatic/jp.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1267 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/nonadiabatic/wcdhc.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.397879 dftpy-2.0.0rc2/src/dftpy/functional/pseudo/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    24427 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/pseudo/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2197 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/pseudo/abstract_pseudo.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2563 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/pseudo/layer_pseudo.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2462 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/pseudo/psp.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1559 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/pseudo/recpot.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     4062 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/pseudo/upf.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     3373 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/pseudo/usp.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     3025 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/pseudo/xml.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    21594 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/semilocal_xc.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     3708 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/total_functional.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     8582 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/functional/xc.json
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    23130 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/grid.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    18815 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/interface.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1168 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/inverter.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     4668 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/ions.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2785 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/linear_solver.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    15076 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/math_utils.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1420 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/mixer.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.397879 dftpy-2.0.0rc2/src/dftpy/mpi/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      248 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/mpi/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2923 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/mpi/mp_mpi4py.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2614 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/mpi/mp_serial.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    10314 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/mpi/mpi.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1202 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/mpi/utils.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.397879 dftpy-2.0.0rc2/src/dftpy/old/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     6326 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/old/atom.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     6062 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/old/cell.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     7471 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/old/coord.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     5114 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/old/pbc_array.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1821 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/old/system.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    21103 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/optimization.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    10612 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/optimize.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.401878 dftpy-2.0.0rc2/src/dftpy/properties/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)       71 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/properties/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      251 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/properties/potential.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.401878 dftpy-2.0.0rc2/src/dftpy/td/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)        0 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/td/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     8385 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/td/casida.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     6571 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/td/hamiltonian.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2661 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/td/interface.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1934 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/td/operator.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     5104 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/td/predictor_corrector.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.401878 dftpy-2.0.0rc2/src/dftpy/td/propagator/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1092 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/td/propagator/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1748 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/td/propagator/abstract_propagator.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     6806 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/td/propagator/crank_nicholson.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2017 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/td/propagator/taylor.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)    13333 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/td/real_time_runner.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1215 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/td/utils.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     3458 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/time_data.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.401878 dftpy-2.0.0rc2/src/dftpy/utils/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1703 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/utils/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     9932 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/utils/utils.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.401878 dftpy-2.0.0rc2/src/dftpy/visualize/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      991 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/visualize/__init__.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      217 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/visualize/ase_viewer.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      822 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/visualize/ipv_viewer.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     1099 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/visualize/jupyter.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     2778 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/visualize/mpl_viewer.py
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      868 2022-10-13 18:11:07.000000 dftpy-2.0.0rc2/src/dftpy/visualize/vesta_viewer.py
+drwxrwxr-x   0 sxc       (1000) sxc       (1000)        0 2022-10-13 20:29:53.393879 dftpy-2.0.0rc2/src/dftpy.egg-info/
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      982 2022-10-13 20:29:53.000000 dftpy-2.0.0rc2/src/dftpy.egg-info/PKG-INFO
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)     6434 2022-10-13 20:29:53.000000 dftpy-2.0.0rc2/src/dftpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)        1 2022-10-13 20:29:53.000000 dftpy-2.0.0rc2/src/dftpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)      239 2022-10-13 20:29:53.000000 dftpy-2.0.0rc2/src/dftpy.egg-info/requires.txt
+-rw-rw-r--   0 sxc       (1000) sxc       (1000)        6 2022-10-13 20:29:53.000000 dftpy-2.0.0rc2/src/dftpy.egg-info/top_level.txt
```

### Comparing `dftpy-2.0.0/.gitlab-ci.yml` & `dftpy-2.0.0rc2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/LICENSE.txt` & `dftpy-2.0.0rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/PKG-INFO` & `dftpy-2.0.0rc2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: dftpy
-Version: 2.0.0
+Version: 2.0.0rc2
 Summary: Python3 packages for Density Functional Theory
 Home-page: http://dftpy.rutgers.edu
 Author: Pavanello Research Group
 Author-email: m.pavanello@rutgers.edu
 License: MIT
+Description: # DFTpy's Manual and Tutorials
+        
+        See [DFTpy's website](http://dftpy.rutgers.edu) for details.
+        
+        
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
+Provides-Extra: all
 Provides-Extra: libxc
-Provides-Extra: upf
 Provides-Extra: mpi
-Provides-Extra: all
-License-File: LICENSE.txt
-
-# DFTpy's Manual and Tutorials
-
-See [DFTpy's website](http://dftpy.rutgers.edu) for details.
-
-
-
-
+Provides-Extra: upf
```

### Comparing `dftpy-2.0.0/doc/Makefile` & `dftpy-2.0.0rc2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/gen_doc.py` & `dftpy-2.0.0rc2/doc/gen_doc.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/make.bat` & `dftpy-2.0.0rc2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/conf.py` & `dftpy-2.0.0rc2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/contact.rst` & `dftpy-2.0.0rc2/doc/source/contact.rst`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/faq.rst` & `dftpy-2.0.0rc2/doc/source/faq.rst`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/index.rst` & `dftpy-2.0.0rc2/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/install.rst` & `dftpy-2.0.0rc2/doc/source/install.rst`

 * *Files 25% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 ============
 Installation
 ============
 
 Requirements
 ============
 
-* Python_ >= 3.6
-* NumPy_ >= 1.8.0
-* SciPy_ >= 0.18.0
-* ASE_  >= 3.22.0
-* xmltodict_ >= 0.12.0
+* Python_ 3.6 or newer
+* NumPy_ 1.8.0 or newer
+* SciPy_ 0.10 or newer
 
 Optional:
 
 * pylibxc_ (for using exchange-correlation functionals other than LDA)
 * pyFFTW_  (for Fast Fourier Transform)
+* ASE_  (for dealing with structures, dynamics, and more)
+* xmltodict_ (For UPF pseudopotential)
 * upf_to_json_ (For UPF pseudopotential)
 * mpi4py_ (MPI for python)
 * mpi4py-fft_ (Fast Fourier Transforms with MPI)
 
 .. _Python: https://www.python.org/
 .. _NumPy: https://docs.scipy.org/doc/numpy/reference/
 .. _SciPy: https://docs.scipy.org/doc/scipy/reference/
@@ -29,35 +29,34 @@
 .. _ASE: https://gitlab.com/ase/ase
 .. _mpi4py: https://bitbucket.org/mpi4py/mpi4py
 .. _mpi4py-fft: https://bitbucket.org/mpi4py/mpi4py-fft
 .. _xmltodict: https://github.com/martinblech/xmltodict
 .. _upf_to_json: https://github.com/simonpintarelli/upf_to_json
 
 
-Installation with pip
-=====================
-
-Using pip can easy install the release version of DFTpy from `PyPI <https://pypi.org/project/dftpy>`_::
-
-    $ python -m pip install dftpy
-
 Installation from source
 ========================
 
-You can get the source from `gitlab <https://gitlab.com/pavanello-research-group/dftpy>`_.::
+You can get the source from `gitlab <https://gitlab.com/pavanello-research-group/dftpy.git>`_.
+
+Git clone:
+----------
 
     $ git clone https://gitlab.com/pavanello-research-group/dftpy.git
-    $ python -m pip install ./dftpy
 
-Or in one line::
-    
-    $ python -m pip install git+https://gitlab.com/pavanello-research-group/dftpy.git
 
+Environment
+^^^^^^^^^^^
+
+    Add ``dftpy/src`` to your `PYTHONPATH` environment variable.
+
+Installation
+^^^^^^^^^^^^
 
-You also can install all the optional packages with::
+    Alternatively, you can install ``DFTpy`` with ``python -m pip install .``
 
-    $ python -m pip install ./dftpy[all]
+    You also can install all the optional packages with ``python -m pip install .[all]``
 
 
 .. note::
 
     Because ``DFTpy`` still under active development, non-backward-compatible changes can happen at any time. Please, clone the lastest release often.
```

### Comparing `dftpy-2.0.0/doc/source/ofdft.rst` & `dftpy-2.0.0rc2/doc/source/ofdft.rst`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/static/dftpy.ico` & `dftpy-2.0.0rc2/doc/source/static/dftpy.ico`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/static/dftpy.jpg` & `dftpy-2.0.0rc2/doc/source/static/dftpy.jpg`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/static/dftpy.png` & `dftpy-2.0.0rc2/doc/source/static/dftpy.png`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/static/dftpy_new_bkg.png` & `dftpy-2.0.0rc2/doc/source/static/dftpy_new_bkg.png`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/templates/breadcrumbs.html` & `dftpy-2.0.0rc2/doc/source/templates/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/templates/footer.html` & `dftpy-2.0.0rc2/doc/source/templates/footer.html`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/tutorials/jupyter/density.png` & `dftpy-2.0.0rc2/doc/source/tutorials/jupyter/density.png`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/tutorials/jupyter/ions.png` & `dftpy-2.0.0rc2/doc/source/tutorials/jupyter/ions.png`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/tutorials/jupyter/movie.gif` & `dftpy-2.0.0rc2/doc/source/tutorials/jupyter/movie.gif`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/tutorials/ofdft/nvt.py` & `dftpy-2.0.0rc2/doc/source/tutorials/ofdft/nvt.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/tutorials/ofdft/relax.py` & `dftpy-2.0.0rc2/doc/source/tutorials/ofdft/relax.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/tutorials/ofdft/relax.rst` & `dftpy-2.0.0rc2/doc/source/tutorials/ofdft/relax.rst`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/tutorials/tddft/propagate.ini` & `dftpy-2.0.0rc2/doc/source/tutorials/tddft/propagate.ini`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/doc/source/tutorials/tddft/propagate.rst` & `dftpy-2.0.0rc2/doc/source/tutorials/tddft/propagate.rst`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/Al_fde_rho.pp` & `dftpy-2.0.0rc2/examples/DATA/Al_fde_rho.pp`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/Al_lda.oe01.recpot` & `dftpy-2.0.0rc2/examples/DATA/Al_lda.oe01.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/As_lda.oe04.recpot` & `dftpy-2.0.0rc2/examples/DATA/As_lda.oe04.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/GaAs.cif` & `dftpy-2.0.0rc2/examples/DATA/GaAs.cif`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/GaAs.vasp` & `dftpy-2.0.0rc2/examples/DATA/GaAs.vasp`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/GaAs_random.vasp` & `dftpy-2.0.0rc2/examples/DATA/GaAs_random.vasp`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/GaAs_random.xsf` & `dftpy-2.0.0rc2/examples/DATA/GaAs_random.xsf`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/Ga_lda.oe04.recpot` & `dftpy-2.0.0rc2/examples/DATA/Ga_lda.oe04.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/Mg8.vasp` & `dftpy-2.0.0rc2/examples/DATA/Mg8.vasp`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/Mg_OEPP_PZ.UPF` & `dftpy-2.0.0rc2/examples/DATA/Mg_OEPP_PZ.UPF`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/Mg_cluster.vasp` & `dftpy-2.0.0rc2/examples/DATA/Mg_cluster.vasp`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/Mg_lda.oe01.recpot` & `dftpy-2.0.0rc2/examples/DATA/Mg_lda.oe01.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/al.gga.recpot` & `dftpy-2.0.0rc2/examples/DATA/al.gga.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/al.lda.lps` & `dftpy-2.0.0rc2/examples/DATA/al.lda.lps`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/al.lda.psp` & `dftpy-2.0.0rc2/examples/DATA/al.lda.psp`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/al.lda.recpot` & `dftpy-2.0.0rc2/examples/DATA/al.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/al.lda.upf` & `dftpy-2.0.0rc2/examples/DATA/al.lda.upf`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/as.lda.recpot` & `dftpy-2.0.0rc2/examples/DATA/as.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/ase_opt.traj` & `dftpy-2.0.0rc2/examples/DATA/ase_opt.traj`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/cd.vasp` & `dftpy-2.0.0rc2/examples/DATA/cd.vasp`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/ga.lda.recpot` & `dftpy-2.0.0rc2/examples/DATA/ga.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/in.lda.recpot` & `dftpy-2.0.0rc2/examples/DATA/in.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/initial_atoms_md.traj` & `dftpy-2.0.0rc2/examples/DATA/initial_atoms_md.traj`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/li.lda.recpot` & `dftpy-2.0.0rc2/examples/DATA/li.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/md.traj` & `dftpy-2.0.0rc2/examples/DATA/md.traj`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/mg.lda.recpot` & `dftpy-2.0.0rc2/examples/DATA/mg.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/p.lda.recpot` & `dftpy-2.0.0rc2/examples/DATA/p.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/sb.lda.recpot` & `dftpy-2.0.0rc2/examples/DATA/sb.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/si.gga.recpot` & `dftpy-2.0.0rc2/examples/DATA/si.gga.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/DATA/si.lda.recpot` & `dftpy-2.0.0rc2/examples/DATA/si.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/md/test_ase_npt.py` & `dftpy-2.0.0rc2/examples/md/test_ase_npt.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 #-----------------------------------------------------------------------
 from ase.lattice.cubic import FaceCenteredCubic
 from ase.md.npt import NPT
 from ase.md.velocitydistribution import MaxwellBoltzmannDistribution
 from ase.io.trajectory import Trajectory
 from ase import units
 
-from dftpy.config.config import DefaultOption, OptionFormat, PrintConf
+from dftpy.config.config import DefaultOption, ConfSpecialFormat, PrintConf
 from dftpy.api.api4ase import DFTpyCalculator
 np.random.seed(8888)
 
 ############################## initial config ##############################
 conf = DefaultOption()
 conf["PATH"]["pppath"] = os.environ.get("DFTPY_DATA_PATH")
 conf["PP"]["Al"] = "al.lda.recpot"
 conf["OPT"]["method"] = "TN"
 conf["KEDF"]["kedf"] = "WT"
 conf["JOB"]["calctype"] = "Energy Force Stress"
 conf["OUTPUT"]["time"] = False
 conf["OUTPUT"]["stress"] = False
-conf = OptionFormat(conf)
+conf = ConfSpecialFormat(conf)
 PrintConf(conf)
 calc = DFTpyCalculator(config=conf, mp = mp)
 # -----------------------------------------------------------------------
 """
 Ref :
     https://wiki.fysik.dtu.dk/ase/ase/md.html#module-ase.md
     https://wiki.fysik.dtu.dk/ase/_modules/ase/md/npt.html#NPT
@@ -60,15 +60,15 @@
 def printenergy(a=atoms):
     global step, interval
     epot = a.get_potential_energy() / len(a)
     ekin = a.get_kinetic_energy() / len(a)
     spot = a.get_stress()
     press = np.sum(spot[:3]) / 3.0
     sprint(
-        "Step={:<8d} Epot={:.5f} Ekin={:.5f} T={:.3f} Etot={:.5f} Press={:.5f}".format(
+        "Step={:<d} Epot={:.5f} Ekin={:.5f} T={:.3f} Etot={:.5f} Press={:.5f}".format(
             step, epot, ekin, ekin / (1.5 * units.kB), epot + ekin, press / units.GPa
         )
     )
     step += interval
 
 def check_stop():
     if os.path.isfile('dftpy_stopfile'): exit()
```

### Comparing `dftpy-2.0.0/examples/md/test_ase_nvt.py` & `dftpy-2.0.0rc2/examples/md/test_ase_nvt.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 #-----------------------------------------------------------------------
 from ase.lattice.cubic import FaceCenteredCubic
 from ase.md.langevin import Langevin
 from ase.md.velocitydistribution import MaxwellBoltzmannDistribution
 from ase.io.trajectory import Trajectory
 from ase import units
 
-from dftpy.config.config import DefaultOption, OptionFormat, PrintConf
+from dftpy.config.config import DefaultOption, ConfSpecialFormat, PrintConf
 from dftpy.api.api4ase import DFTpyCalculator
 np.random.seed(8888)
 
 ############################## initial config ##############################
 conf = DefaultOption()
 conf["PATH"]["pppath"] = os.environ.get("DFTPY_DATA_PATH")
 conf["PP"]["Al"] = "al.lda.recpot"
 conf["OPT"]["method"] = "TN"
 conf["KEDF"]["kedf"] = "WT"
 conf["JOB"]["calctype"] = "Energy Force"
 conf["OUTPUT"]["time"] = False
-conf = OptionFormat(conf)
+conf = ConfSpecialFormat(conf)
 PrintConf(conf)
 calc = DFTpyCalculator(config=conf, mp = mp)
 # -----------------------------------------------------------------------
 """
 Ref :
     https://wiki.fysik.dtu.dk/ase/ase/md.html#module-ase.md
 """
```

### Comparing `dftpy-2.0.0/examples/md/test_ase_nvt_nh.py` & `dftpy-2.0.0rc2/examples/md/test_ase_nvt_nh.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 #-----------------------------------------------------------------------
 from ase.lattice.cubic import FaceCenteredCubic
 from ase.md.npt import NPT
 from ase.md.velocitydistribution import MaxwellBoltzmannDistribution
 from ase.io.trajectory import Trajectory
 from ase import units
 
-from dftpy.config.config import DefaultOption, OptionFormat, PrintConf
+from dftpy.config.config import DefaultOption, ConfSpecialFormat, PrintConf
 from dftpy.api.api4ase import DFTpyCalculator
 np.random.seed(8888)
 
 ############################## initial config ##############################
 conf = DefaultOption()
 conf["PATH"]["pppath"] = os.environ.get("DFTPY_DATA_PATH")
 conf["PP"]["Al"] = "al.lda.recpot"
 conf["OPT"]["method"] = "TN"
 conf["KEDF"]["kedf"] = "WT"
 conf["JOB"]["calctype"] = "Energy Force"
 conf["OUTPUT"]["time"] = False
-conf = OptionFormat(conf)
+conf = ConfSpecialFormat(conf)
 PrintConf(conf)
 calc = DFTpyCalculator(config=conf, mp = mp)
 # -----------------------------------------------------------------------
 """
 Ref :
     https://wiki.fysik.dtu.dk/ase/ase/md.html#module-ase.md
     https://wiki.fysik.dtu.dk/ase/_modules/ase/md/npt.html#NPT
```

### Comparing `dftpy-2.0.0/examples/ofdft/config.ini` & `dftpy-2.0.0rc2/examples/ofdft/config.ini`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/ofdft/isolate.ini` & `dftpy-2.0.0rc2/examples/ofdft/isolate.ini`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/ofdft/optim.py` & `dftpy-2.0.0rc2/examples/ofdft/optim.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/ofdft/simple.py` & `dftpy-2.0.0rc2/examples/ofdft/simple.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/relax/test_ase_opt.py` & `dftpy-2.0.0rc2/examples/relax/test_ase_opt.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/test/common.py` & `dftpy-2.0.0rc2/examples/test/common.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/test/test_ase_md.py` & `dftpy-2.0.0rc2/examples/test/test_ase_md.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 #!/usr/bin/env python3
 import os
 import unittest
 import numpy as np
 
+# from dftpy.config.config import DefaultOption, ConfSpecialFormat
 from dftpy.config import DefaultOption, OptionFormat
+from dftpy.interface import OptimizeDensityConf
 from dftpy.api.api4ase import DFTpyCalculator
 import pytest
 
 
 class Test(unittest.TestCase):
     def test_md(self):
         pytest.importorskip("ase")
+        from ase.lattice.cubic import FaceCenteredCubic
         from ase.md.langevin import Langevin
         from ase.md.verlet import VelocityVerlet
         from ase.md.velocitydistribution import MaxwellBoltzmannDistribution
         from ase.io.trajectory import Trajectory
         from ase import units
         from ase.io import write, read
         dftpy_data_path = os.environ.get('DFTPY_DATA_PATH')
```

### Comparing `dftpy-2.0.0/examples/test/test_ase_opt.py` & `dftpy-2.0.0rc2/examples/test/test_ase_opt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 #!/usr/bin/env python3
 import os
 import unittest
 import numpy as np
 import pytest
 
-from dftpy.config import DefaultOption, OptionFormat
+from dftpy.config.config import DefaultOption, ConfSpecialFormat
+from dftpy.interface import OptimizeDensityConf
 from dftpy.api.api4ase import DFTpyCalculator
 
 class Test(unittest.TestCase):
     def test_opt(self):
         pytest.importorskip("ase")
+        from ase.calculators.interface import Calculator
+        from ase.lattice.cubic import FaceCenteredCubic
         from ase.optimize import BFGS, LBFGS, FIRE
         from ase.optimize.sciopt import SciPyFminBFGS, SciPyFminCG
         from ase.constraints import StrainFilter, UnitCellFilter
         from ase.io.trajectory import Trajectory
         from ase import units
         from ase.io import read, write
         dftpy_data_path = os.environ.get('DFTPY_DATA_PATH')
         conf = DefaultOption()
         conf['PATH']['pppath'] = os.environ.get('DFTPY_DATA_PATH')
         conf['PP']['Al'] = 'al.lda.recpot'
         conf['JOB']['calctype'] = 'Energy Force Stress'
         conf['OPT']['method'] = 'TN'
         conf['OUTPUT']['stress'] = False
         conf['EXC']['xc'] = 'LDA'
-        conf = OptionFormat(conf)
+        conf = ConfSpecialFormat(conf)
         path = os.environ.get('DFTPY_DATA_PATH')
         atoms = read(path+'/'+'fcc.vasp')
         calc = DFTpyCalculator(config = conf)
         atoms.calc = calc
         af = StrainFilter(atoms)
         opt = SciPyFminCG(af)
         opt.run(fmax = 0.001)
         atoms_final = read(filename=dftpy_data_path+'/ase_opt.traj',format='traj')
         self.assertTrue(np.isclose(atoms.positions, atoms_final.positions, atol=1.e-3).all())
 
-
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `dftpy-2.0.0/examples/test/test_ase_pmg_io.py` & `dftpy-2.0.0rc2/examples/test/test_ase_pmg_io.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/test/test_density_opt.py` & `dftpy-2.0.0rc2/examples/test/test_density_opt.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/test/test_ewald.py` & `dftpy-2.0.0rc2/examples/test/test_ewald.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/test/test_field.py` & `dftpy-2.0.0rc2/examples/test/test_field.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/test/test_functional.py` & `dftpy-2.0.0rc2/examples/test/test_functional.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/test/test_functional_LibXC.py` & `dftpy-2.0.0rc2/examples/test/test_functional_LibXC.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 #!/usr/bin/env python3
 import os
 import unittest
 import numpy as np
 import pytest
 
 from dftpy.functional import Functional
-from dftpy.functional.semilocal_xc import LibXC
+from dftpy.functional.semilocal_xc import LibXC, PBE
 from dftpy.formats import io
 
 
 class Test(unittest.TestCase):
     def test_libxc_lda(self):
         pytest.importorskip("pylibxc")
         dftpy_data_path = os.environ.get('DFTPY_DATA_PATH')
         rho_r = io.read_density(dftpy_data_path + "/Al_fde_rho.pp")
-        thefuncclass = Functional(type='XC', name='LDA', libxc=False)
+        thefuncclass = Functional(type='XC',
+                                  name='LDA',
+                                  libxc=False)
         func2 = thefuncclass.compute(rho_r)
-        func1 = LibXC(density=rho_r, libxc =['lda_x', 'lda_c_pz'])
+        func1 = LibXC(density=rho_r,
+                   x_str='lda_x',
+                   c_str='lda_c_pz')
         a = func2.energy
         b = func1.energy
         self.assertTrue(np.allclose(a, b))
 
     def test_libxc_pbe(self):
         pytest.importorskip("pylibxc")
         dftpy_data_path = os.environ.get('DFTPY_DATA_PATH')
         rho_r = io.read_density(dftpy_data_path + "/Al_fde_rho.pp")
-        Functional_LibXC = LibXC(density=rho_r, libxc =['gga_x_pbe', 'gga_c_pbe'])
-        Functional_LibXC2 = Functional(type='XC', xc ='PBE').compute(rho_r)
+        Functional_LibXC = LibXC(density=rho_r,
+                              x_str='gga_x_pbe',
+                              c_str='gga_c_pbe')
+        Functional_LibXC2 = PBE(rho_r)
         self.assertTrue(
             np.isclose(Functional_LibXC2.energy, Functional_LibXC.energy))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `dftpy-2.0.0/examples/test/test_grid.py` & `dftpy-2.0.0rc2/examples/test/test_grid.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/test/test_linear_solver.py` & `dftpy-2.0.0rc2/examples/test/test_linear_solver.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/test/test_mpi_grid.py` & `dftpy-2.0.0rc2/examples/test/test_mpi_grid.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/test/test_pme.py` & `dftpy-2.0.0rc2/examples/test/test_pme.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,21 +17,21 @@
         ions, rho, _ = io.read_all(dftpy_data_path + "/Al_fde_rho.pp")
         PP_list = {'Al': dftpy_data_path + "/Al_lda.oe01.recpot"}
         grid = rho.grid
 
         PSEUDO = LocalPseudo(grid=grid, ions=ions, PP_list=PP_list, PME=False)
         func = PSEUDO(rho)
         IE_Energy = func.energy
-        IE_Force = PSEUDO.forces(rho)
+        IE_Force = PSEUDO.force(rho)
         IE_Stress = PSEUDO.stress(rho, energy=IE_Energy)
 
         PSEUDO = LocalPseudo(grid=grid, ions=ions, PP_list=PP_list, PME=True)
         func = PSEUDO(rho)
         IE_Energy_PME = func.energy
-        IE_Force_PME = PSEUDO.forces(rho)
+        IE_Force_PME = PSEUDO.force(rho)
         IE_Stress_PME = PSEUDO.stress(rho, energy=IE_Energy_PME)
 
         print('IE energy', IE_Energy, IE_Energy_PME)
         self.assertTrue(np.isclose(IE_Energy, IE_Energy_PME, atol=1.E-4))
         print('IE forces', IE_Force, IE_Force_PME)
         self.assertTrue(np.allclose(IE_Force, IE_Force_PME, atol=1.E-4))
         print('IE stress', IE_Stress, IE_Stress_PME)
```

### Comparing `dftpy-2.0.0/examples/test/test_propagator.py` & `dftpy-2.0.0rc2/examples/test/test_propagator.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/test/test_read_pp.py` & `dftpy-2.0.0rc2/examples/test/test_read_pp.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/examples/test/test_snpy.py` & `dftpy-2.0.0rc2/examples/test/test_snpy.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/scripts/convertPP.py` & `dftpy-2.0.0rc2/scripts/convertPP.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/scripts/convert_den.py` & `dftpy-2.0.0rc2/scripts/convert_den.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/scripts/convert_td.py` & `dftpy-2.0.0rc2/scripts/convert_td.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/scripts/invert` & `dftpy-2.0.0rc2/scripts/invert`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/scripts/opt_layer_pseudo.py` & `dftpy-2.0.0rc2/scripts/opt_layer_pseudo.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/scripts/quadrupole.py` & `dftpy-2.0.0rc2/scripts/quadrupole.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/scripts/rtc_runner` & `dftpy-2.0.0rc2/scripts/rtc_runner`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/scripts/test_layer_pseudo.py` & `dftpy-2.0.0rc2/scripts/test_layer_pseudo.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/setup.py` & `dftpy-2.0.0rc2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,23 +31,21 @@
 description = "Python3 packages for Density Functional Theory"
 
 with open('README.md') as fh :
     long_description = fh.read()
 
 scripts = ['scripts/dftpy']
 extras_require = {
-        'libxc' : [
-            'pylibxc2; python_version<"3.10"',
-            # 'pylibxc @ git+https://gitlab.com/libxc/libxc.git;python_version>"3.9"',
-            ],
-        'upf' : ['upf_to_json'],
+        'libxc' : ['pylibxc2'],
+        'upf' : ['xmltodict', 'upf_to_json'],
         'mpi': ['mpi4py', 'mpi4py-fft'],
         'all' : [
-            'pylibxc2; python_version<"3.10"',
-            # 'pylibxc @ git+https://gitlab.com/libxc/libxc.git;python_version>"3.9"',
+            'pylibxc2',
+            'ase>=3.21.1',
+            'xmltodict',
             'upf_to_json',
             'mpi4py',
             'mpi4py-fft',
             'pyfftw',
             ],
         }
```

### Comparing `dftpy-2.0.0/src/dftpy/api/api4ase.py` & `dftpy-2.0.0rc2/src/dftpy/api/api4ase.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,17 +42,18 @@
             self.atoms["lattice"] = lattice.copy()
             self.atoms["positions"] = pos.copy()
             #
             ions = Ions.from_ase(atoms)
             #
             if self.results is not None and self.config["MATH"]["reuse"]:
                 config, others = ConfigParser(self.config, ions=ions, rhoini=self.results["density"], pseudo=pseudo, grid=grid, mp = self.mp)
+                results = OptimizeDensityConf(config, others["ions"], others["field"], others["E_v_Evaluator"], others["nr2"])
             else:
                 config, others = ConfigParser(self.config, ions=ions, pseudo=pseudo, grid=grid, mp = self.mp)
-            results = OptimizeDensityConf(config, **others)
+                results = OptimizeDensityConf(config, others["ions"], others["field"], others["E_v_Evaluator"], others["nr2"])
             self.results = results
         energy = self.results["energypotential"]["TOTAL"].energy * ENERGY_CONV["Hartree"]["eV"]
         energy = self.results["density"].grid.mp.asum(energy)
         return energy
 
     def get_forces(self, atoms):
         if self.check_restart(atoms):
```

### Comparing `dftpy-2.0.0/src/dftpy/api/dftd4.py` & `dftpy-2.0.0rc2/src/dftpy/api/dftd4.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/config/config.py` & `dftpy-2.0.0rc2/src/dftpy/config/config.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/config/config_entry.py` & `dftpy-2.0.0rc2/src/dftpy/config/config_entry.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/config/configentries.json` & `dftpy-2.0.0rc2/src/dftpy/config/configentries.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992766203703702%*

 * *Differences: {"'OPT'": "{'method': {'type': 'str'}, 'algorithm': {'type': 'str', 'options': 'EMM, RMM', "*

 * *          "'comment': 'The direct minimization method : Energy (EMM) or Residual (RMM).', delete: "*

 * *          "['note']}}"}*

```diff
@@ -465,19 +465,18 @@
         "copy": {
             "default": "NONADIABATIC",
             "type": "str"
         }
     },
     "OPT": {
         "algorithm": {
-            "comment": "Direct energy minimization method (EMM), direct residual minimization method (RMM), and one-orbital ensemble self-consistent field (`OESCF <https://pubs.acs.org/doi/full/10.1021/acs.jpclett.1c00716>`_).",
+            "comment": "The direct minimization method : Energy (EMM) or Residual (RMM).",
             "default": "EMM",
-            "note": "In `OESCF` solver, the :ref:`kedf<kedf-kedf>` has to contains full `vW` functional.",
-            "options": "EMM, RMM, OESCF",
-            "type": "ustr"
+            "options": "EMM, RMM",
+            "type": "str"
         },
         "c1": {
             "comment": "The wolfe parameters `c1`",
             "default": 0.0001,
             "options": "",
             "type": "float"
         },
@@ -522,15 +521,15 @@
             "options": "",
             "type": "int"
         },
         "method": {
             "comment": "The density optimization method.",
             "default": "CG-HS",
             "options": "TN, LBFGS, CG-HS, CG-DY, CG-CD, CG-LS, CG-FR, CG-PR",
-            "type": "ustr"
+            "type": "str"
         },
         "vector": {
             "comment": "The scheme to deal with search direction.",
             "default": "Orthogonalization",
             "options": "Orthogonalization, Scaling",
             "type": "str"
         },
```

### Comparing `dftpy-2.0.0/src/dftpy/constants.py` & `dftpy-2.0.0rc2/src/dftpy/constants.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/cui/main.py` & `dftpy-2.0.0rc2/src/dftpy/cui/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,18 +44,18 @@
         elif "Casida" in config["JOB"]["task"]:
             CasidaRunner(config, others["field"], others["E_v_Evaluator"])
         elif "Diagonalize" in config["JOB"]["task"]:
             DiagonalizeRunner(config, others["field"], others["ions"], others["E_v_Evaluator"])
         elif "Inversion" in config["JOB"]["task"]:
             InvertRunner(config, others["field"], others["E_v_Evaluator"])
         else:
-            OptimizeDensityConf(config, **others)
+            OptimizeDensityConf(config, others["ions"], others["field"], others["E_v_Evaluator"], others["nr2"])
 
         TimeData.End("TOTAL")
-        TimeData.output(config, sort=1)
+        TimeData.output(config)
         sprint("-" * 80)
     sprint("#" * 80)
     sprint("DFTpy {} Finished on : {}".format(__version__, time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())))
 
 def main():
     import sys
     from dftpy.mpi.utils import sprint
```

### Comparing `dftpy-2.0.0/src/dftpy/ewald.py` & `dftpy-2.0.0rc2/src/dftpy/ewald.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,50 +189,53 @@
         mask = self.get_Qarray_mask(l123A)
         Qarray[l123A[0][mask], l123A[1][mask], l123A[2][mask]] += Mn_multi.ravel()[mask]
         # Qarray = DirectField(self.grid,griddata_3d=Qarray,rank=1)
         return Qarray
 
 
 class ewald(object):
-    def __init__(self, precision=1.0e-8, ions=None, rho=None, grid = None, verbose=False, BsplineOrder=10, PME=False, Bspline=None, **kwargs):
+    def __init__(self, precision=1.0e-8, ions=None, rho=None, grid = None, verbose=False, BsplineOrder=10, PME=False, Bspline=None):
         """
-        This computes Ewald contributions to the energy.
+        This computes Ewald contributions to the energy given a DirectField rho.
         INPUT: precision  float, should be bigger than the machine precision and
                           smaller than single precision.
                ions       Ions class array.
+               rho        DirectField, the electron density needed to evaluate
+                          the singular parts of the energy.
                verbose    optional, wanna sprint stuff?
         """
 
         self.precision = precision
 
         self.verbose = verbose
 
         self.grid = grid
+        self.rho = rho
 
         if ions is not None:
             self.ions = ions
         else:
             raise AttributeError("Must pass ions to Ewald")
 
         if self.grid is None:
-            if rho is not None :
-                self.grid =rho.grid
+            if self.rho is not None :
+                self.grid =self.rho.grid
             else:
-                raise AttributeError("Must pass grid or rho to Ewald")
+                raise AttributeError("Must pass rho to Ewald")
 
         self.mp = self.grid.mp
 
         gmax = self.Get_Gmax(self.grid)
         eta = self.Get_Best_eta(self.precision, gmax, self.ions)
         # eta = 0.2
         self.eta = eta
         self.order = BsplineOrder
 
-        self.PME = PME
-        if self.PME:
+        self.usePME = PME
+        if self.usePME:
             if Bspline is None:
                 self.Bspline = CBspline(ions=self.ions, grid=self.grid, order=self.order)
             else:
                 self.Bspline = Bspline
         self._energy = None
         self._forces = None
         self._stress = None
@@ -484,15 +487,15 @@
         return energy
 
     @property
     @timer()
     def energy(self):
         if self._energy is None:
             e_corr = self.Energy_corr()
-            if self.PME:
+            if self.usePME:
                 e_real = self.Energy_real_fast2()
                 e_rec = self.Energy_rec_PME()
             else:
                 e_real = self.Energy_real()
                 e_rec = self.Energy_rec()
 
             e_corr /= self.mp.comm.size
@@ -508,29 +511,29 @@
         return self._energy
 
     @property
     @timer()
     def forces(self):
         if self._forces is None:
             Ewald_Forces = self.Forces_real()
-            if self.PME:
+            if self.usePME:
                 f_rec = self.Forces_rec_PME()
             else:
                 f_rec = self.Forces_rec()
             Ewald_Forces += f_rec
             self._forces = Ewald_Forces
         return self._forces
 
     @property
     @timer()
     def stress(self):
         if self._stress is None:
 
             Ewald_Stress = self.Stress_real()
-            if self.PME:
+            if self.usePME:
                 s_rec = self.Stress_rec_PME()
             else:
                 s_rec = self.Stress_rec()
 
             Ewald_Stress += s_rec
 
             if self.verbose:
@@ -778,15 +781,15 @@
                 Mn.append(Bspline.calc_Mn(Up[j] - np.floor(Up[j])))
             Mn_multi = np.einsum(
                 "i, j, k -> ijk", self.ions.charges[i] * Mn[0][1:], Mn[1][1:], Mn[2][1:]
             )
             l123A = np.mod(np.floor(Up).astype(np.int32).reshape((3, 1)) - ixyzA, nr.reshape((3, 1)))
             mask = self.Bspline.get_Qarray_mask(l123A)
             Qarray[l123A[0][mask], l123A[1][mask], l123A[2][mask]] += Mn_multi.ravel()[mask]
-        return DirectField(self.grid, data=Qarray)
+        return DirectField(self.grid, griddata_3d=np.reshape(Qarray, np.shape(self.rho)), rank=1)
 
     @timer()
     def Energy_rec_PME(self):
         QarrayF = self.Bspline.PME_Qarray
         # bm = self.Bspline.bm
         # method 1
         strf = QarrayF.fft()
@@ -893,15 +896,15 @@
                 sfactor[k] *= 2.0 / gg * (1 + gg / (4.0 * self.eta))
                 if i == j:
                     sfactor[k] -= 1.0
                 k += 1
 
         Stmp = np.einsum("ijk, ijkl->l", strf_sq * np.exp(-gg / (4.0 * self.eta)) * invgg, sfactor)
 
-        Stmp = Stmp.real * 2.0 * np.pi / self.grid.volume ** 2 / self.grid.dV ** 2
+        Stmp = Stmp.real * 2.0 * np.pi / self.grid.volume ** 2 / self.rho.grid.dV ** 2
         # G = 0 term
         sum = self.ions.get_ncharges()
         S_g0 = sum ** 2 * 4.0 * np.pi * (1.0 / (4.0 * self.eta * self.grid.volume ** 2) / 2.0) / self.mp.comm.size
         k = 0
         S_rec = np.zeros((3, 3))
         for i in range(3):
             for j in range(i, 3):
@@ -949,15 +952,15 @@
                     "i, i->", strf_sq[mask] * np.exp(-gg[mask] / (4.0 * self.eta)) * invgg[mask], sfactor[k][mask]
                 ).real
                 )
                 k += 1
 
         # Stmp =np.einsum('ijk, ijkl->l', strf_sq*np.exp(-gg/(4.0*self.eta))*invgg, sfactor)
 
-        Stmp = Stmp.real * 2.0 * np.pi / self.grid.volume ** 2 / self.grid.dV ** 2
+        Stmp = Stmp.real * 2.0 * np.pi / self.grid.volume ** 2 / self.rho.grid.dV ** 2
         # G = 0 term
         sum = self.ions.get_ncharges()
         S_g0 = sum ** 2 * 4.0 * np.pi * (1.0 / (4.0 * self.eta * self.grid.volume ** 2) / 2.0) / self.mp.comm.size
         k = 0
         S_rec = np.zeros((3, 3))
         for i in range(3):
             for j in range(i, 3):
```

### Comparing `dftpy-2.0.0/src/dftpy/fft.py` & `dftpy-2.0.0rc2/src/dftpy/fft.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/field.py` & `dftpy-2.0.0rc2/src/dftpy/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,25 +133,18 @@
         return self.grid.cell
 
 
 class DirectField(BaseField):
     spl_order = 3
 
     def __new__(cls, grid, memo="", rank=1, data = None, order = 'C', cplx=False, **kwargs):
-        if hasattr(grid, 'get_direct'): grid = grid.get_direct()
         if not isinstance(grid, DirectGrid):
             raise TypeError("the grid argument is not an instance of DirectGrid")
         obj = super().__new__(
             cls, grid, memo="", rank=rank, data = data, order = order, cplx = cplx, **kwargs)
-        #
-        obj.init_options = locals()
-        for k in ['__class__', 'cls', 'obj', 'kwargs', 'grid', 'data'] :
-            obj.init_options.pop(k, None)
-        # obj.init_options.update(kwargs)
-        #
         obj._N = None
         obj.spl_coeffs = None
         obj._cplx = cplx
         if obj.mp.is_mpi :
             from dftpy.mpi.mp_mpi4py import mpi_fft
             obj.fft_object = mpi_fft(obj.grid)
         elif not obj._cplx and np.all(obj.grid.nr == obj.grid.nrG):  # Can only use numpy.fft
@@ -620,32 +613,21 @@
         from dftpy.formats import io as dftpy_io
         dftpy_io.write(filename, data=self, ions=ions, format=format, **kwargs)
 
     def read(self, filename, format=None, **kwargs):
         from dftpy.formats import io as dftpy_io
         self[:] = dftpy_io.read_density(filename, format=format, **kwargs)
 
-    def cut_highg(self, g2max = None):
-        recip = self.fft().cut_highg(g2max)
-        return recip.ifft()
-
 
 class ReciprocalField(BaseField):
     def __new__(cls, grid, memo="", rank=1, data = None, order = 'C', cplx=False, **kwargs):
-        if hasattr(grid, 'get_reciprocal'): grid = grid.get_reciprocal()
         if not isinstance(grid, ReciprocalGrid):
             raise TypeError("the grid argument is not an instance of ReciprocalGrid")
         obj = super().__new__(
             cls, grid, memo="", rank=rank, data = data, order = order, cplx = True, **kwargs)
-        #
-        obj.init_options = locals()
-        for k in ['__class__', 'cls', 'obj', 'kwargs', 'grid', 'data'] :
-            obj.init_options.pop(k, None)
-        # obj.init_options.update(kwargs)
-        #
         obj.spl_coeffs = None
         obj._cplx = cplx
         if obj.mp.is_mpi :
             from dftpy.mpi.mp_mpi4py import mpi_ifft
             obj.ifft_object = mpi_ifft(obj.grid)
         elif not obj._cplx and np.all(obj.grid.nrG == obj.grid.nrR):  # Can only use numpy.fft
             obj.ifft_object = np.fft.ifftn
@@ -757,15 +739,7 @@
         return self._cplx
 
     @cplx.setter
     def cplx(self, value):
         self._cplx = value
         if self._cplx and not self.grid.full :
             self.grid.full = True
-
-    def cut_highg(self, g2max = None):
-        if self.rank == 1:
-            self[~self.grid.get_gmask(g2max)] = 0.0
-        else:
-            for i in range(self.rank):
-                self[i][~self.grid.get_gmask(g2max)] = 0.0
-        return self
```

### Comparing `dftpy-2.0.0/src/dftpy/formats/ase_io.py` & `dftpy-2.0.0rc2/src/dftpy/formats/ase_io.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/formats/cube.py` & `dftpy-2.0.0rc2/src/dftpy/formats/cube.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/formats/den.py` & `dftpy-2.0.0rc2/src/dftpy/formats/den.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/formats/io.py` & `dftpy-2.0.0rc2/src/dftpy/formats/io.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import os
 from collections import namedtuple
 from importlib import import_module
-from dftpy.grid import DirectGrid
 from dftpy.field import DirectField
-from dftpy.mpi import SerialComm, MP
+from dftpy.mpi import SerialComm
 from dftpy.ions import Ions
 
 ioformat = namedtuple('ioformat', ['format', 'module', 'read', 'write', 'kind'])
 iounkeys = ['mp', 'comm', 'kind', 'data_type', 'grid', 'names']
 
 IOFormats= {
             "snpy"    : ioformat('snpy', 'dftpy.formats.snpy'  , 'read_snpy', 'write_snpy', ['ions', 'data', 'all']),
             "xsf"     : ioformat('xsf' , 'dftpy.formats.xsf'   , 'read_xsf' , 'write_xsf' , ['ions', 'data', 'all']),
+            "pp"      : ioformat('qepp', 'dftpy.formats.qepp'  , 'read_qepp', 'write_qepp', ['ions', 'data', 'all']),
             "qepp"    : ioformat('qepp', 'dftpy.formats.qepp'  , 'read_qepp', 'write_qepp', ['ions', 'data', 'all']),
             "cube"    : ioformat('cube', 'dftpy.formats.cube'  , 'read_cube', 'write_cube', ['ions', 'data', 'all']),
             "den"     : ioformat('den' , 'dftpy.formats.den'   , 'read_den' , 'write_den' , ['data']),
             "xyz"     : ioformat('xyz' , 'dftpy.formats.xyz'   , 'read_xyz' , 'write_xyz' , ['ions']),
+            "extxyz"  : ioformat('xyz' , 'dftpy.formats.xyz'   , 'read_xyz' , 'write_xyz' , ['ions']),
             "vasp"    : ioformat('vasp', 'dftpy.formats.vasp'  , 'read_vasp', 'write_vasp', ['ions']),
+            "poscar"  : ioformat('vasp', 'dftpy.formats.vasp'  , 'read_vasp', 'write_vasp', ['ions']),
+            "contcar" : ioformat('vasp', 'dftpy.formats.vasp'  , 'read_vasp', 'write_vasp', ['ions']),
             "ase"     : ioformat('ase' , 'dftpy.formats.ase_io', 'read_ase' , 'write_ase' , ['ions']),
             "pmg"     : ioformat('pmg' , 'dftpy.formats.pmg_io', 'read_pmg' , 'write_pmg' , ['ions']),
+            "pymatgen": ioformat('pmg' , 'dftpy.formats.pmg_io', 'read_pmg' , 'write_pmg' , ['ions']),
         }
 
-IOFormats['pp'] = IOFormats['qepp']
-IOFormats['extxyz'] = IOFormats['xyz']
-IOFormats['poscar'] = IOFormats['vasp']
-IOFormats['contcar'] = IOFormats['vasp']
-IOFormats['pymatgen'] = IOFormats['pmg']
-
 def guessType(infile, **kwargs):
     return guess_format(infile, **kwargs)
 
 def guess_format(infile, **kwargs):
     basename = os.path.basename(infile).lower()
     ext = os.path.splitext(infile)[1].lower()
     format = IOFormats.get(basename, None)
@@ -61,80 +59,39 @@
             if not iof.write or func is None : raise AttributeError("%s format not support write" % iof.format)
             iof = iof._replace(write = func)
     except Exception as e:
         raise e
 
     return iof
 
-def read(infile, format=None, kind='ions', ecut=None, driver=None, mp=None, grid=None, **kwargs):
+def read(infile, format=None, kind='ions', driver=None, **kwargs):
     if driver is None :
         driver = get_io_driver(infile, format, mode = 'r')
     elif isinstance(driver, str) :
         for key in iounkeys :
             if key in kwargs : kwargs.pop(key)
         driver = get_io_driver(infile, driver, mode = 'r')
     #
-    if mp is None :
-        if grid is None :
-            mp = MP()
-        else :
-            mp = grid.mp
-
     if hasattr(driver, 'read') :
-        if mp.is_root or driver.format == "snpy": # only snpy format support MPI-IO
-            if driver.format in ['ase', 'pmg'] :
-                values = driver.read(infile, format=format, **kwargs)
-            else :
-                values = driver.read(infile, kind=kind, mp=mp, grid=grid, **kwargs)
-        else :
-            values = [None, ]*3
+        values = driver.read(infile, format=format, **kwargs)
     else :
         raise AttributeError(f"Sorry, not support {driver} driver")
-
-    ions = data = info = None
-    if kind == 'ions' :
-        ions = values
-    elif kind == 'data' :
-        data = values
-    else :
+    #
+    if kind == 'all' :
         if 'ions' not in driver.kind :
-            data = values
+            values = (None, values, None)
         elif 'data' not in driver.kind :
-            ions = values
+            values = (values, None, None)
         elif len(values) == 2 :
-            ions, data = values
-        elif len(values) == 3 :
-            ions, data, info = values
-        else :
+            values = *values, None
+        elif len(values) != 3 :
             raise AttributeError(f"Sorry, the {driver} driver should only return 3 values.")
-    #-----------------------------------------------------------------------
-    if mp.size > 1 and driver.format != "snpy":
-        ions_options = getattr(ions, 'init_options', 0)
-        ions_options = mp.comm.bcast(ions_options)
-        if ions_options :
-            ions = Ions(**ions_options)
-        grid_options = getattr(getattr(data, 'grid', 0), 'init_options', 0)
-        grid_options = mp.comm.bcast(grid_options)
-        if grid_options :
-            grid_options['mp'] = mp
-            grid = DirectGrid(**grid_options)
-            data_options = getattr(data, 'init_options', 0)
-            data_options = mp.comm.bcast(data_options)
-            data2 = DirectField(grid=grid, **data_options)
-            grid.scatter(data, out = data2)
-            data = data2
-        info = mp.comm.bcast(info)
-    #-----------------------------------------------------------------------
-    if ecut and hasattr(data, 'grid') : data.grid.ecut = ecut
-    if kind == 'ions' :
-        values = ions
-    elif kind == 'data' :
-        values = data
-    else :
-        values = (ions, data, info)
+    if kind == 'data' :
+        if len(values) == 2 or len(values) == 3 :
+            values = values[1]
     return values
 
 def write(outfile, ions = None, data = None, information = None, format = None, comm = None, driver = None, **kwargs):
     if isinstance(data, Ions):
         if ions is None or isinstance(ions, DirectField):
             ions, data = data, ions
         else :
```

### Comparing `dftpy-2.0.0/src/dftpy/formats/npy.py` & `dftpy-2.0.0rc2/src/dftpy/formats/npy.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/formats/pmg_io.py` & `dftpy-2.0.0rc2/src/dftpy/formats/pmg_io.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/formats/qepp.py` & `dftpy-2.0.0rc2/src/dftpy/formats/qepp.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,27 +36,27 @@
                 at = np.zeros((3, 3), dtype=float)
                 for ilat in range(3):
                     linesplt = filepp.readline().split()
                     at[ilat] = np.asarray(linesplt, dtype=float)
                 at *= celldm[0]
             else:
                 at = self.celldm2at(ibrav, celldm)
+            grid = DirectGrid(lattice=at, nr=nrx, full=full)
 
             # gcutm, dual, ecut, plot_num
             gcutm, dual, ecut, plot_num = (float(x) for x in filepp.readline().split())
             plot_num = int(plot_num)
             # filepp.readline()
             # gcutm, dual, ecut, plot_num = 1.0, 1.0, 1.0, 0
             self.cutoffvars["ibrav"] = ibrav
             self.cutoffvars["celldm"] = celldm
             self.cutoffvars["gcutm"] = gcutm
             self.cutoffvars["dual"] = dual
             self.cutoffvars["ecut"] = ecut
             self.cutoffvars["plot_num"] = plot_num
-            grid = DirectGrid(lattice=at, nr=nrx, full=full, ecut=ecut)
 
             # ntyp
             atm = []
             zv = np.empty(ntyp, dtype=float)
             zval = {}
             for ity in range(ntyp):
                 linesplt = filepp.readline().split()
```

### Comparing `dftpy-2.0.0/src/dftpy/formats/snpy.py` & `dftpy-2.0.0rc2/src/dftpy/formats/snpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,17 @@
         if key == 1 : # read cell
             lattice = npy.read(fh, single = True)
         elif key == 2 : # read numbers
             numbers = npy.read(fh, single = True)
         elif key == 3 : # read coordinates
             pos = npy.read(fh, single = True)
             ions = Ions(numbers=numbers, positions=pos, cell=lattice)
-            if kind == 'ions' : break
+            if kind == 'ions' :
+                if isinstance(fname, str): fh.close()
+                return ions
         elif key == 4 : # read volumetric data
             if mp.size == 1 :
                 data = npy.read(fh, single=True)
                 shape = data.shape
                 if len(shape) == 4 :
                     rank = shape[0]
                     shape = shape[1:]
@@ -121,17 +123,15 @@
                 elif not(np.all(shape == grid.nrR) or np.all(shape == grid.nrG)):
                     raise AttributeError("The shape {} is not match with grid {} (or {})".format(shape, grid.nrR, grid.nrG))
                 order = 'F' if fortran_order else 'C'
                 data = DirectField(grid=grid, rank=rank, order = order)
                 npy._read_value(fh, data, datarep=datarep, fortran_order=fortran_order)
 
     if isinstance(fname, str): fh.close()
-    if kind == 'ions' :
-        return ions
-    elif kind == 'data' :
+    if len(desc) == 1 :
         return data
     else :
         return ions, data, None
 
 def read_snpy(fname, **kwargs):
     return read(fname, **kwargs)
```

### Comparing `dftpy-2.0.0/src/dftpy/formats/vasp.py` & `dftpy-2.0.0rc2/src/dftpy/formats/vasp.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/formats/xsf.py` & `dftpy-2.0.0rc2/src/dftpy/formats/xsf.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,19 +158,21 @@
         be added as needed.
         So far it can:
             - write the ions
             - write the 1D/2D/3D grid data
         """
 
         with open(self.filexsf, "w") as fileout:
-            if units.lower() == 'angstrom' : ions = ions.to_ase()
+            if units.lower() == 'angstrom' :
+                ions = ions.to_ase()
             self._write_header(fileout, title)
             self._write_cell(fileout, ions.cell)
             self._write_coord(fileout, ions)
-            self._write_datagrid(fileout, data, data_type = data_type, units = units)
+            # the data always in 'angstrom' units
+            self._write_datagrid(fileout, data, data_type = data_type)
 
         return
 
     def read(self, kind="all", full=False, **kwargs):
         return read_xsf(self.filexsf, kind=kind, full=full, **kwargs)
 
     def _write_header(self, fileout, title):
@@ -185,27 +187,26 @@
 
     def _write_coord(self, fileout, ions):
         mywrite(fileout, "PRIMCOORD", True)
         mywrite(fileout, (len(ions.positions), 1), True)
         for i in range(len(ions.positions)):
             mywrite(fileout, (ions.symbols[i], ions.positions[i]), True)
 
-    def _write_datagrid(self, fileout, plot, data_type = 'density', units = 'angstrom', **kwargs):
+    def _write_datagrid(self, fileout, plot, data_type = 'density', **kwargs):
         ndim = plot.span  # 2D or 3D grid?
         if ndim < 2:
             return  # XSF format doesn't support one data grids
         val_per_line = 5
         rank = plot.rank
         grid = plot.grid
         if rank == 1 :
             plot = [plot]
         data = []
         for p in plot :
-            values = p.get_values_flatarray(pad=1, order="F")
-            if units == 'angstrom' : values /= Units.Bohr ** 3
+            values = p.get_values_flatarray(pad=1, order="F") / Units.Bohr ** 3
             if data_type == 'potential' :
                 values = values * Units.Ha
             data.append(values)
 
         mywrite(fileout, "BEGIN_BLOCK_DATAGRID_{}D".format(ndim), True)
         mywrite(fileout, "{}d_datagrid_{}".format(ndim, data_type), True)
         for i, values in enumerate(data) :
@@ -215,16 +216,15 @@
                 mywrite(fileout, (grid.nr[0] + 1, grid.nr[1] + 1, grid.nr[2] + 1), True)
             elif ndim == 2:
                 mywrite(fileout, (grid.nr[0] + 1, grid.nr[1] + 1), True)
             mywrite(
                 fileout, origin, True
             )  # TODO, there might be an actual origin if we're dealing with a custom cut of the grid
             for ilat in range(ndim):
-                latt = grid.lattice[ilat]
-                if units == 'angstrom' : latt = latt * Units.Bohr
+                latt = grid.lattice[ilat] * Units.Bohr
                 mywrite(fileout, latt, True)
 
             nnr = len(values)
             nlines = nnr // val_per_line
             for iline in range(nlines):
                 igrid = iline * val_per_line
                 mywrite(fileout, values[igrid : igrid + val_per_line], True)
```

### Comparing `dftpy-2.0.0/src/dftpy/formats/xyz.py` & `dftpy-2.0.0rc2/src/dftpy/formats/xyz.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     line = fh.readline().strip()
     p = re.compile(r'(Lattice)'+r'\s*=\s*["\{]([^"\{\}]+)["\}]\s*')
     m = p.match(line)
     if m is None :
         lattice = np.zeros((3, 3))
     else :
         lattice = np.fromstring(m.group(2), dtype=float, sep=" ")
-        lattice = np.asarray(lattice).reshape((3, 3))
+        lattice = np.asarray(lattice).reshape((3, 3)).T
     symbols = []
     pos = []
     for i in range(natom):
         line = fh.readline().split()
         symbols.append(line[0])
         pos.append(list(map(float, line[1:4])))
     pos = np.asarray(pos)
```

### Comparing `dftpy-2.0.0/src/dftpy/functional/__init__.py` & `dftpy-2.0.0rc2/src/dftpy/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/abstract_functional.py` & `dftpy-2.0.0rc2/src/dftpy/functional/abstract_functional.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 # functional class (output handler) in output
 
 # local imports
 # from dftpy.mpi import sprint
 
 # general python imports
 from abc import ABC, abstractmethod
-from dftpy.functional.functional_output import FunctionalOutput
 
 
 class AbstractFunctional(ABC):
     @abstractmethod
     def __init__(self):
         pass
 
     def __repr__(self):
-        name = getattr(self, 'name', self.__class__.__name__)
-        rep = name + ', ' + self.__dict__.__repr__()
+        rep = self.name + ', ' + self.__dict__.__repr__()
         return rep
 
     def __call__(self, rho, *args, **kwargs):
         return self.compute(rho, *args, **kwargs)
 
     @abstractmethod
     def compute(self, rho, *args, **kwargs):
```

### Comparing `dftpy-2.0.0/src/dftpy/functional/external_potential.py` & `dftpy-2.0.0rc2/src/dftpy/functional/external_potential.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,10 +28,7 @@
     def compute(self, rho, calcType={"E", "V"}, **kwargs):
         pot = self.v
         if 'E' in calcType:
             ene = np.einsum("ijk, ijk->", self.v, rho) * self.v.grid.dV
         else:
             ene = 0
         return FunctionalOutput(name="ext", energy=ene, potential=pot)
-
-    def potential(self):
-        return self.v
```

### Comparing `dftpy-2.0.0/src/dftpy/functional/functional_output.py` & `dftpy-2.0.0rc2/src/dftpy/functional/functional_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,15 @@
         ]
 
     def __iter__(self):
         for key in self.attr_list:
             if hasattr(self, key):
                 yield key, getattr(self, key)
 
-    def sum(self, other = None):
-        if other is None : return self.copy()
+    def sum(self, other):
         if self.name == other.name:
             name = self.name
         else:
             name = self.name + other.name
         result = FunctionalOutput(name=name)
         for key, value in self:
             if hasattr(other, key):
```

### Comparing `dftpy-2.0.0/src/dftpy/functional/hartree.py` & `dftpy-2.0.0rc2/src/dftpy/functional/hartree.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/kedf/__init__.py` & `dftpy-2.0.0rc2/src/dftpy/functional/kedf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import copy
 
 import numpy as np
 
 from dftpy.functional.abstract_functional import AbstractFunctional
 from dftpy.functional.functional_output import FunctionalOutput, ZeroFunctional
 from dftpy.functional.kedf.fp import FP
-from dftpy.functional.kedf.gga import GGA, GGA_KEDF_list, GGAFs, MGGA, MGGA_KEDF_list
+from dftpy.functional.kedf.gga import GGA, GGA_KEDF_list, GGAFs
 from dftpy.functional.kedf.hc import HC, revHC
 from dftpy.functional.kedf.lwt import LWT, LMGP, LMGPA, LMGPG
-from dftpy.functional.kedf.mgp import MGP, MGPA, MGPG, MGP0
+from dftpy.functional.kedf.mgp import MGP, MGPA, MGPG
 from dftpy.functional.kedf.sm import SM
 from dftpy.functional.kedf.tf import TF, TTF, ThomasFermiStress
 from dftpy.functional.kedf.vw import vW, vonWeizsackerStress
 from dftpy.functional.kedf.wt import WT, WTStress
 from dftpy.functional.semilocal_xc import LibXC
 from dftpy.mpi import sprint
 from dftpy.utils import name2functions
@@ -25,15 +25,14 @@
 
 KEDFEngines= {
         "NONE": ZeroFunctional,
         "TF": TF,
         "VW": vW,
         "LKT": LKT,
         "GGA": GGA,
-        "MGGA": MGGA,
         "WT-NL": WT,
         "SM-NL": SM,
         "FP-NL": FP,
         "MGP-NL": MGP,
         "MGPA-NL": MGPA,
         "MGPG-NL": MGPG,
         "LWT-NL": LWT,
@@ -56,16 +55,14 @@
         "LWT": ("TF", "VW", "LWT-NL"),
         "LMGP": ("TF", "VW", "LMGP-NL"),
         "LMGPA": ("TF", "VW", "LMGPA-NL"),
         "LMGPG": ("TF", "VW", "LMGPG-NL"),
         "HC": ("TF", "VW", "HC-NL"),
         "REVHC": ("TF", "VW", "REVHC-NL"),
         "TTF": TF,
-        "MGP0-NL": MGP0,
-        "MGP0": ("TF", "VW", "MGP0-NL"),
         }
 
 KEDFEngines_Stress = {
     "TF": ThomasFermiStress,
     "VW": vonWeizsackerStress,
     "WT-NL": WTStress,
     "X_TF_Y_VW": ("TF", "VW"),
@@ -104,26 +101,15 @@
 
     def compute(self, density, calcType={"E", "V"}, name=None, kedf = None, split=False, **kwargs):
         if kedf : name = kedf
         if name is None : name = self.name
         name = name.upper()
         options = copy.deepcopy(self.options)
         options.update(kwargs)
-        #-----------------------------------------------------------------------
-        k_str = options.pop('k_str', None) # For GGA functional
-        if name.startswith('GGA_'):
-            k_str = name[4:]
-            options['mgga'] = False
-            name = 'GGA'
-        elif name.startswith('MGGA_'):
-            k_str = name[5:]
-            options['mgga'] = True
-            name = 'MGGA'
-        options['functional'] = k_str
-        #-----------------------------------------------------------------------
+        options['functional'] = options.pop('k_str', None) # For GGA functional
         options = {k :v for k, v in options.items() if v is not None}
         functional = {}
         if density.ndim > 3:
             nspin = density.rank
             rhos = density*nspin
         else :
             nspin = 1
```

### Comparing `dftpy-2.0.0/src/dftpy/functional/kedf/fp.py` & `dftpy-2.0.0rc2/src/dftpy/functional/kedf/fp.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/kedf/gga.py` & `dftpy-2.0.0rc2/src/dftpy/functional/kedf/gga.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from dftpy.math_utils import PowerInt
 from dftpy.time_data import timer
 
 __all__ = ["GGA", "GGAFs", "GGA_KEDF_list"]
 
 
 def s_with_tkf0(function):
-    r'''
+    '''
     Decorator for functionals with a defination of s=\grad\rho / tkf0 / (\rho)^(4/3)
     Parameters
     ----------
     function
 
     Returns
     -------
@@ -37,30 +37,30 @@
         return results
 
     return wrapper
 
 
 @s_with_tkf0
 def LKTmVW(ss: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{luo2018simple}
     '''
     exp_1 = np.exp(-params[0] * ss)
     exp_2 = np.exp(-2.0 * params[0] * ss)
     F = 2.0 * exp_1 / (1.0 + exp_2)
     results = {'F': F}
     if 'V' in calcType:
         dFds2 = - params[0] * (1.0 - exp_2) / (1.0 + exp_2) * F / ss
         results.update({'dFds2': dFds2})
 
     return results
 
 
 def DK(s: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{garcia2007kinetic} (8)
     '''
     x = s * s / (72 * C_TF)
     Fa = 9.0 * params[5] * x ** 4 + params[2] * x ** 3 + params[1] * x ** 2 + params[0] * x + 1.0
     Fb = params[5] * x ** 3 + params[4] * x ** 2 + params[3] * x + 1.0
     F = Fa / Fb
     results = {'F': F}
@@ -71,15 +71,15 @@
         dFds2 /= 36.0 * C_TF
         results.update({'dFds2': dFds2})
 
     return results
 
 
 def LLP(s: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{garcia2007kinetic} (9)[!x]
     \cite{gotz2009performance} (18)
     '''
     bs = CBRT_TWO * s
     bs2 = bs * bs
     Fa = params[0] * bs2
     Fb = 1.0 + params[1] * bs * np.arcsinh(bs)
@@ -92,15 +92,15 @@
         dFds2 *= CBRT_TWO * CBRT_TWO
         results.update({'dFds2': dFds2})
 
     return results
 
 
 def OL(s: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{gotz2009performance} (16)
     \cite{gotz2009performance} (17)
     '''
     tol2 = 1.0e-8
     F = 1.0 + s * s / 72.0 / C_TF + params[0] / C_TF * s / (1 + params[1] * 4 * s)
     results = {'F': F}
     if "V" in calcType:
@@ -109,15 +109,15 @@
         dFds2[mask] += params[0] / C_TF / PowerInt((1 + params[1] * 4 * s[mask]), 2) / s[mask]
         results.update({'dFds2': dFds2})
 
     return results
 
 
 def THAK(s: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{garcia2007kinetic} (12),
     \cite{gotz2009performance} (22),
     \cite{hfofke} (15)[!x]
     '''
     tol2 = 1.0e-8
     bs = CBRT_TWO * s
     bs2 = bs * bs
@@ -139,15 +139,15 @@
         dFds2 *= CBRT_TWO * CBRT_TWO
         results.update({'dFds2': dFds2})
 
     return results
 
 
 def B86A(s: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{garcia2007kinetic} (13)
     '''
     bs = CBRT_TWO * s
     bs2 = bs * bs
     Fa = params[0] * bs2
     Fb = 1.0 + params[1] * bs2
     F = 1.0 + Fa / Fb
@@ -156,15 +156,15 @@
         dFds2 = 2 * params[0] / (Fb * Fb) * (CBRT_TWO * CBRT_TWO)
         results.update({'dFds2': dFds2})
 
     return results
 
 
 def B86B(s: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{garcia2007kinetic} (14)
     '''
     bs = CBRT_TWO * s
     bs2 = bs * bs
     Fa = params[0] * bs2
     Fb = PowerInt((1.0 + params[1] * bs2), 4, 5)
     F = 1.0 + Fa / Fb
@@ -173,15 +173,15 @@
         dFds2 = (2 * params[0] * (params[1] * bs2 + 5.0)) / (5 * (1.0 + params[1] * bs2) * Fb) * (CBRT_TWO * CBRT_TWO)
         results.update({'dFds2': dFds2})
 
     return results
 
 
 def DK87(s: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{garcia2007kinetic} (15)
     '''
     bs = CBRT_TWO * s
     bs2 = bs * bs
     Fa = params[0] * bs2 * (1 + params[1] * bs)
     Fb = 1.0 + params[2] * bs2
     F = 1.0 + Fa / Fb
@@ -192,15 +192,15 @@
         results.update({'dFds2': dFds2})
 
     return results
 
 
 @s_with_tkf0
 def PW86(ss: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{gotz2009performance} (19)
     '''
     s2 = ss * ss
     s4 = s2 * s2
     s6 = s2 * s4
     Fa = 1.0 + params[0] * s2 + params[1] * s4 + params[2] * s6
     F = np.power(Fa, 1.0 / 15.0)
@@ -210,15 +210,15 @@
         results.update({'dFds2': dFds2})
 
     return results
 
 
 @s_with_tkf0
 def PW910(ss: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{gotz2009performance} (20)
     '''
     s2 = ss * ss
     s4 = s2 * s2
     Fa = (params[1] - params[2] * np.exp(-params[3] * s2)) * s2 - params[5] * s4
     Fb = 1.0 + params[0] * ss * np.arcsinh(params[4] * ss) + params[5] * s4
     F = 1.0 + Fa / Fb
@@ -236,15 +236,15 @@
         results.update({'dFds2': dFds2})
 
     return results
 
 
 @s_with_tkf0
 def PW91(ss: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{lacks1994tests} (16) and
     \cite{garcia2007kinetic} (17)[!x]
     '''
     tol2 = 1.0e-8
     s2 = ss * ss
     s4 = s2 * s2
     Fa = 1.0 + params[0] * ss * np.arcsinh(params[4] * ss) + (params[1] - params[2] * np.exp(-params[3] * s2)) * s2
@@ -274,15 +274,15 @@
         results.update({'dFds2': dFds2})
 
     return results
 
 
 @s_with_tkf0
 def LG94(ss: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{garcia2007kinetic} (18)
     '''
     s2 = ss * ss
     s4 = s2 * s2
     s6 = s4 * s2
     s8 = s4 * s4
     s10 = s4 * s6
@@ -313,15 +313,15 @@
         results.update({'dFds2': dFds2})
 
     return results
 
 
 @s_with_tkf0
 def P92(ss: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{gotz2009performance} (14)
     \cite{gotz2009performance} (15)
     '''
     s2 = ss * ss
     s4 = s2 * s2
     Fa = params[0] + params[1] * s2 + params[2] * s4
     Fb = params[0] + params[3] * s2
@@ -332,15 +332,15 @@
         results.update({'dFds2': dFds2})
 
     return results
 
 
 @s_with_tkf0
 def PBE(ss: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{gotz2009performance} (23)
     \cite{hfofke} (20)
     \cite{hfofke} (32)
     \cite{hfofke} (33)
     '''
     s2 = ss * ss
     Fa = params[1] * s2
@@ -365,15 +365,15 @@
         results.update({'dFds2': dFds2})
 
     return results
 
 
 @s_with_tkf0
 def P82(ss: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{hfofke} (9)
     '''
     s2 = ss * ss
     s6 = s2 * s2 * s2
     Fb = 1 + s6
     F = 1.0 + params[0] * s2 / Fb
     results = {'F': F}
@@ -382,34 +382,34 @@
         results.update({'dFds2': dFds2})
 
     return results
 
 
 @s_with_tkf0
 def VJKS00(ss: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{hfofke} (18)
     '''
     s2 = ss * ss
     s4 = s2 * s2
     s6 = s4 * s2
-    Fa = 1.0 + params[0] * s2 - params[2] * s6
+    Fa = 1.0 + params[0] * s2
     Fb = 1.0 + params[1] * s2 + params[2] * s4
     F = Fa / Fb
     results = {'F': F}
     if "V" in calcType:
-        dFds2 = (2.0 * params[0] - 6.0 * params[2] * s4)/ Fb - (2.0 * params[1] + 4.0 * params[2] * s2)*Fa/(Fb*Fb)
+        dFds2 = (2.0 * params[0]) / Fb - (2.0 * params[1] + 4.0 * params[2] * s2) * Fa / (Fb * Fb)
         results.update({'dFds2': dFds2})
 
     return results
 
 
 @s_with_tkf0
 def VT84F(ss: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
-    r'''
+    '''
     \cite{hfofke} (33)
     '''
     tol2 = 1.0e-8
     s2 = ss * ss
     s2[s2 < tol2] = tol2
     s4 = s2 * s2
     F = (
@@ -485,67 +485,14 @@
     results = {'F': F}
     if "V" in calcType:
         dFds2 = -2.0 * params[0] * Fa + 10.0 / 3.0 * params[1]
         results.update({'dFds2': dFds2})
 
     return results
 
-@s_with_tkf0
-def GE2(ss: DirectField, calcType: Set[str], params: List[float], q: DirectField, **kwargs) -> Dict:
-    s2 = ss * ss
-    F = params[0] + params[1] * s2 + params[2] * q
-    results = {'F': F}
-    if "V" in calcType:
-        dFds2 = 2.0 * params[1]
-        dFdq = params[2]
-        results['dFds2'] = dFds2
-        results['dFdq'] = dFdq
-
-    return results
-
-@s_with_tkf0
-def GE4(ss: DirectField, calcType: Set[str], params: List[float], q: DirectField, **kwargs) -> Dict:
-    results = GE2.__wrapped__(ss, calcType=calcType, params=params[:3], q=q, **kwargs)
-    s2 = ss * ss
-    F = params[3] * q * q + params[4] * q * s2 + params[5] * s2 * s2
-    results['F'] += F
-    if "V" in calcType:
-        dFds2 = 2.0 * params[4] * q + 4.0 * params[5] * s2
-        dFdq = 2.0 * params[3] * q + params[4] * s2
-        results['dFds2'] += dFds2
-        results['dFdq'] += dFdq
-
-    return results
-
-@s_with_tkf0
-def PGSL(ss: DirectField, calcType: Set[str], params: List[float], q: DirectField, **kwargs) -> Dict:
-    s2 = ss * ss
-    Fa = np.exp(-params[1] * s2)
-    F = Fa + q**2*params[0] + 5.0 / 3.0 * params[2] * s2
-    results = {'F': F}
-    if "V" in calcType:
-        dFds2 = -2.0 * params[1] * Fa + 10.0 / 3.0 * params[2]
-        dFdq = 2.0 * params[0] * q
-        results['dFds2'] = dFds2
-        results['dFdq'] = dFdq
-
-    return results
-
-@s_with_tkf0
-def PGSLr(ss: DirectField, calcType: Set[str], params: List[float], q: DirectField, **kwargs) -> Dict:
-    results = PGSL.__wrapped__(ss, calcType=calcType, params=params[2:], q=q, **kwargs)
-    s2 = ss * ss
-    F = -params[0] * q * s2 + params[1] * s2 * s2
-    results['F'] += F
-    if "V" in calcType:
-        dFds2 = -2.0 * params[0] * q + 4.0 * params[1] * s2
-        dFdq = -params[0] * s2
-        results['dFds2'] += dFds2
-        results['dFdq'] += dFdq
-    return results
 
 @s_with_tkf0
 def LKT_legacy(ss: DirectField, calcType: Set[str], params: List[float], **kwargs) -> Dict:
     s2 = ss * ss
     F = np.empty_like(ss)
     dFds2 = np.empty_like(ss)
     mask1 = ss > 100.0
@@ -638,21 +585,14 @@
     "TFVW": TFVW_dict,
     "STV": {"function": STV, "params": [1.0, 1.0, 0.01, 1.0]},
     "PBE2M": {"function": PBE2M, "params": [1.0, 0.2942, 2.0309]},
     "PG": {"function": PG, "params": [0.75, 1.0]},
     # "TEST-TF-APBEK": [1.3, 0.23889, 1.245],
 }
 
-MGGA_KEDF_list = {
-    "GE2": {"function": GE2, "params": [1.0, 5.0/27.0, 20.0/9.0]},
-    "GE4": {"function": GE4, "params": [1.0, 5.0/27.0, 20.0/9.0, 8.0/81.0, -1.0/9.0, 8.0/243.0]},
-    "PGSL": {"function": PGSL, "params": [0.25, 40.0/27.0, 1.0]}, # \beta, \mu, vw
-    "PGSLR": {"function": PGSLr, "params": [0.40, 0.20, 0.25, 40.0/27.0, 1.0]}, # \lambda, \sigma, \beta, \mu, vw
-}
-
 
 # def GGAStress(rho, functional="LKT", energy=None, potential=None, dFds2=None, **kwargs):
 #     """
 #     Not finished.
 #     """
 #     rhom = rho.copy()
 #     tol = 1e-16
@@ -1045,19 +985,21 @@
             dFds2 /= TKF0 * TKF0
 
     elif functional == "VJKS00":  # \cite{hfofke} (18) !something wrong
         ss = s / TKF0
         s2 = ss * ss
         s4 = s2 * s2
         s6 = s4 * s2
-        Fa = 1.0 + params[0] * s2 - params[2] * s6
+        # Fa = 1.0 + params[0] * s2 - params[2] * s6
+        Fa = 1.0 + params[0] * s2
         Fb = 1.0 + params[1] * s2 + params[2] * s4
         F = Fa / Fb
         if "V" in calcType:
-            dFds2 = (2.0 * params[0] - 6.0 * params[2] * s4)/ Fb - (2.0 * params[1] + 4.0 * params[2] * s2)*Fa/(Fb*Fb)
+            # dFds2 = (2.0 * params[0] - 6.0 * params[2] * s4)/ Fb - (2.0 * params[1] + 4.0 * params[2] * s2)*Fa/(Fb*Fb)
+            dFds2 = (2.0 * params[0]) / Fb - (2.0 * params[1] + 4.0 * params[2] * s2) * Fa / (Fb * Fb)
             dFds2 /= TKF0 * TKF0
 
     elif functional == "LC94":  # \cite{hfofke} (16) # same as PW91
         ss = s / TKF0
         s2 = ss * ss
         s4 = s2 * s2
         Fa = 1.0 + params[0] * ss * np.arcsinh(params[4] * ss) + (params[1] - params[2] * np.exp(-params[3] * s2)) * s2
@@ -1243,34 +1185,24 @@
             dFds2 -= 10.0 / 3.0 / TKF0 ** 2 * pa
 
     return F, dFds2
 
 
 @timer()
 def GGA(rho: DirectField, functional: str = "LKT", calcType: Set[str] = {"E", "V"}, split: bool = False, params=None,
-        sigma=None, gga_remove_vw=None, mgga = False, **kwargs):
+        sigma=None, gga_remove_vw=None, **kwargs):
     """
     Interface to compute GGAs internally to DFTpy.
     This is the default way, even though DFTpy can generate some of the GGAs with LibXC.
     Nota Bene: gradient and divergence is done brute force here and in a non-smooth way.
                while the LibXC implementation can be numerically smoothed by changing
                flag='standard' to flag='smooth'. The results with smooth math are
                slightly different.
     """
     functional = functional.upper()
-    if mgga :
-        if functional in MGGA_KEDF_list :
-            Fs_dict = MGGA_KEDF_list[functional]
-        else :
-            raise AttributeError("%s MGGA KEDF to be implemented" % functional)
-    elif functional in GGA_KEDF_list :
-        Fs_dict = GGA_KEDF_list[functional]
-    else :
-        raise AttributeError("%s GGA KEDF to be implemented" % functional)
-    #
     rhom = rho.copy()
     tol = 1e-16
     rhom[rhom < tol] = tol
 
     rho23 = PowerInt(rhom, 2, 3)
     rho53 = rho23 * rhom
     tf = C_TF * rho53
@@ -1281,34 +1213,31 @@
         gradient_flag = 'standard'
     else:
         gradient_flag = 'supersmooth'
     rhoGrad = rho.gradient(flag=gradient_flag, force_real=True, sigma=sigma)
     s = np.sqrt(PowerInt(rhoGrad[0], 2) + PowerInt(rhoGrad[1], 2) + PowerInt(rhoGrad[2], 2)) / rho43
     s[s < tol] = tol
 
-    if mgga :
-        q = rho.laplacian(force_real=True, sigma=sigma)/(TKF0**2)
-        dq0 = -5.0/3.0 * q/rhom
-        dq2 = 1.0/(TKF0**2) / rho53
-    else :
-        q = None
-
+    try:
+        Fs_dict = GGA_KEDF_list[functional]
+    except KeyError:
+        raise AttributeError("%s GGA KEDF to be implemented" % functional)
     if params is None:
         params = Fs_dict["params"]
     else:
         if isinstance(params, (float, int)):
             params = [params]
         len_default_params = len(Fs_dict["params"])
         len_params = len(params)
         if len_params > len_default_params:
             params = params[:len_default_params]
         elif len_params < len_default_params:
             params.extend(Fs_dict["params"][len_params:])
 
-    results = Fs_dict["function"](s, calcType, params, q=q, **kwargs)
+    results = Fs_dict["function"](s, calcType, params, **kwargs)
 
     if gga_remove_vw is not None:
         if isinstance(gga_remove_vw, (int, float)):
             pa = float(gga_remove_vw)
         else:
             pa = 1.0
         vw = TFVW(s, calcType, [0.0, pa], **kwargs)
@@ -1331,20 +1260,18 @@
         p3 = []
         for i in range(3):
             item = tf * results['dFds2'] * rhoGrad[i] / rho83
             p3.append(item.fft())
         g = rhom.grid.get_reciprocal().g
         pot3G = g[0] * p3[0] + g[1] * p3[1] + g[2] * p3[2]
         pot -= (1j * pot3G).ifft(force_real=True)
-
-        if mgga :
-            pot += tf * results['dFdq'] * dq0
-            pot_q2 = tf * results['dFdq'] * dq2
-            pot += pot_q2.laplacian(force_real = True, sigma = sigma)
-
         OutFunctional.potential = pot
+    # np.savetxt('gga.dat', np.c_[rho.ravel(), pot.ravel(), s.ravel(), F.ravel(), dFds2.ravel()])
+
     return OutFunctional
 
-def MGGA(rho: DirectField, functional: str = "LKT", calcType: Set[str] = {"E", "V"}, split: bool = False, params=None,
-        sigma=None, gga_remove_vw=None, mgga = True, **kwargs):
-    return GGA(rho, functional=functional, calcType=calcType, split=split, params=params, sigma=sigma,
-            gga_remove_vw=gga_remove_vw, mgga = True, **kwargs)
+
+def get_gga_p(rho, calcType=["E", "V"], params=None, **kwargs):
+    sigma = kwargs.get('sigma', None)
+    rho53 = rho ** (5.0 / 3.0)
+    p = rho.laplacian(sigma=sigma) / (TKF0 ** 2 * rho53)
+    return p
```

### Comparing `dftpy-2.0.0/src/dftpy/functional/kedf/hc.py` & `dftpy-2.0.0rc2/src/dftpy/functional/kedf/hc.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,15 +353,15 @@
         elif kerneltype == "MGPG":
             KernelTable = MGPKernelTable(eta, maxpoints=maxpoints, symmetrization="Geometric", mp=rho.grid.mp)
         elif kerneltype == "HC":
             KernelTable = HCKernelTable(eta, beta=beta, x=x, y=y, mp=rho.grid.mp)
         # Add MGP kinetic electron
         if lumpfactor is not None:
             sprint('Calculate MGP kinetic electron({})'.format(lumpfactor), comm=rho.mp.comm, level=1)
-            Ne = rho0 * rho.grid.volume
+            Ne = rho0 * rho.grid.Volume
             MGPKernelE = MGPOmegaE(q, Ne, lumpfactor)
             KE_kernel_saved["MGPKernelE"] = MGPKernelE
         # Different method to interpolate the kernel
         if order > 1:
             KE_kernel_saved["KernelTable"] = splrep(eta, KernelTable, k=order)
             KernelDerivTable = splev(eta, KE_kernel_saved["KernelTable"], der=1) * (-1.0 * eta)
             KE_kernel_saved["KernelDeriv"] = splrep(eta, KernelDerivTable, k=order)
@@ -379,14 +379,15 @@
     # -----------------------------------------------------------------------
     # kwargs['functional'] = 'HC'
     # kwargs['params'] = [0.01]
     # one_point_potential_energy(rho, alpha=alpha, beta=beta, etamax=etamax, ratio=ratio, nsp=nsp, kdd=kdd, delta=delta, interp=interp, calcType=calcType, ke_kernel_saved = KE_kernel_saved, **kwargs)
     # -----------------------------------------------------------------------
     return NL
 
+@timer()
 def revHC(
         rho,
         x=1.0,
         y=1.0,
         sigma=None,
         interp="hermite",
         kerneltype="HC",
```

### Comparing `dftpy-2.0.0/src/dftpy/functional/kedf/kernel.py` & `dftpy-2.0.0rc2/src/dftpy/functional/kedf/kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,41 +326,43 @@
     """
     The WT Kernel
     """
     tkf = 2.0 * (3.0 * rho0 * np.pi ** 2) ** (1.0 / 3.0)
     cTF = 0.3 * (3.0 * np.pi ** 2) ** (2.0 / 3.0)
     factor = 5.0 / (9.0 * alpha * beta * rho0 ** (alpha + beta - 5.0 / 3.0))
     factor *= cTF
-    y = 1.0 # always remove whole vW
     return LindhardFunction(q / tkf, x, y) * factor
 
 
 def SMKernel(q, rho0, x=1.0, y=1.0, alpha=0.5, beta=0.5):
     """
     The SM Kernel
     """
     return WTKernel(q, rho0, x, y, alpha, beta)
+    tkf = 2.0 * (3.0 * rho0 * np.pi ** 2) ** (1.0 / 3.0)
+    cTF = 0.3 * (3.0 * np.pi ** 2) ** (2.0 / 3.0)
+    factor = 1.0 / (2.0 * alpha ** 2 * rho0 ** (2.0 * alpha - 2))
+    factor *= cTF
+    return LindhardFunction(q / tkf, x, y) * factor
 
 
 def WTKernelTable(eta, x=1.0, y=1.0, alpha=5.0 / 6.0, beta=5.0 / 6.0):
     """
     Tip : In this version, this is only work for alpha = beta = 5.0/6.0
     """
     # factor =1.2*np.pi**2/(3.0*np.pi**2)**(1.0/3.0)
     # factor = 5.0 / (9.0 * alpha * beta) * (0.3 * (3.0  *  np.pi ** 2) ** (2.0/3.0))
     factor = 4.0 / 5.0 * 0.3 * (3.0 * np.pi ** 2) ** (2.0 / 3.0)
-    y = 1.0 # always remove whole vW
     return LindhardFunction(eta, x, y) * factor
 
 
 def WTKernelDerivTable(eta, x=1.0, y=1.0, alpha=5.0 / 6.0, beta=5.0 / 6.0):
     factor = 5.0 / (9.0 * alpha * beta)
     cTF = 0.3 * (3.0 * np.pi ** 2) ** (2.0 / 3.0)
     factor *= cTF
-    y = 1.0 # always remove whole vW
     return LindhardDerivative(eta, y) * factor
 
 
 def LWTKernel(q, rho0, KernelTable, etamax=1000.0):
     """
     Create the LWT kernel for given rho0 and Kernel Table
     """
@@ -401,15 +403,15 @@
         raise AttributeError("Wrong type of KernelTable")
     Kernel[cond1] = limit
     if q[0, 0, 0] < ZERO:
         Kernel[0, 0, 0] = 0.0
     return Kernel
 
 
-def MGPOmegaE(q, Ne=1, lumpfactor=0.2, revke = True):
+def MGPOmegaE(q, Ne=1, lumpfactor=0.2):
     """
     """
     c = 1.0
     b = None
     if isinstance(lumpfactor, list):
         a = lumpfactor[0]
         if len(lumpfactor) > 1:
@@ -424,23 +426,21 @@
         b = a
 
     qflag = False
     if q[0, 0, 0] < ZERO:
         qflag = True
         q[0, 0, 0] = 1.0
     gg = q ** 2
-    if revke :
-        corr = 4 * np.pi * sp.erf(c * gg) ** 2 * a * np.exp(-gg * b) / gg
-    else :
-        # Same as the formular in MGP
-        corr = 4 * np.pi * sp.erf(c * q) ** 2* a * np.exp(-gg * b) / gg
-        corr *= 3.0/5.0
+    corr = 4 * np.pi * sp.erf(c * gg) ** 2 * a * np.exp(-gg * b) / gg
+    # corr = 4 * np.pi * sp.erf(c * q) ** 2* a * np.exp(-gg * b) / gg + 0.001*np.exp(-0.1*(gg-1.5)**2)
     if qflag:
         q[0, 0, 0] = 0.0
         corr[0, 0, 0] = 0.0
+    # Same as the formular in MGP
+    corr /= 1.2
     return corr
 
 
 def SmoothKernel(q, rho0, x=1.0, y=1.0, alpha=5.0 / 6.0, beta=5.0 / 6.0):
     """
     The WT Kernel
     """
@@ -448,15 +448,14 @@
     cTF = 0.3 * (3.0 * np.pi ** 2) ** (2.0 / 3.0)
     factor = 5.0 / (9.0 * alpha * beta * rho0 ** (alpha + beta - 5.0 / 3.0))
     factor *= cTF
     # -----------------------------------------------------------------------
     coef = 4.0
     factor = factor * np.exp(-(q ** 2) / (coef ** 2 * (tkf / 2.0) ** 2))
     # -----------------------------------------------------------------------
-    y = 1.0 # always remove whole vW
     return LindhardFunction(q / tkf, x, y) * factor
 
 
 @timer()
 def HCKernelTable(eta, beta=2.0 / 3.0, x=1.0, y=1.0, KernelTable=None, mp=None):
     """
     The HC Kernel
```

### Comparing `dftpy-2.0.0/src/dftpy/functional/kedf/lkt.py` & `dftpy-2.0.0rc2/src/dftpy/functional/kedf/lkt.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/kedf/lwt.py` & `dftpy-2.0.0rc2/src/dftpy/functional/kedf/lwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,15 +542,15 @@
         elif kerneltype == "MGPA":
             KernelTable = MGPKernelTable(eta, maxpoints=maxpoints, symmetrization="Arithmetic", mp=rho.grid.mp)
         elif kerneltype == "MGPG":
             KernelTable = MGPKernelTable(eta, maxpoints=maxpoints, symmetrization="Geometric", mp=rho.grid.mp)
         # Add MGP kinetic electron
         if lumpfactor is not None:
             # sprint('Calculate MGP kinetic electron({})'.format(lumpfactor), rho.mp.comm, level=1)
-            Ne = rho0 * rho.grid.volume
+            Ne = rho0 * rho.grid.Volume
             MGPKernelE = MGPOmegaE(q, Ne, lumpfactor)
             KE_kernel_saved["MGPKernelE"] = MGPKernelE
         # Different method to interpolate the kernel
         if order > 1:
             KE_kernel_saved["KernelTable"] = splrep(eta, KernelTable, k=order)
             KernelDerivTable = splev(eta, KE_kernel_saved["KernelTable"], der=1) * (-1.0 * eta)
             KE_kernel_saved["KernelDeriv"] = splrep(eta, KernelDerivTable, k=order)
```

### Comparing `dftpy-2.0.0/src/dftpy/functional/kedf/mgp.py` & `dftpy-2.0.0rc2/src/dftpy/functional/kedf/mgp.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from dftpy.functional.functional_output import FunctionalOutput
 from dftpy.functional.kedf.kernel import MGPKernel, MGPOmegaE
 from dftpy.functional.kedf.wt import WTPotential, WTEnergyDensity
 from dftpy.mpi import sprint
 from dftpy.time_data import timer
 
-__all__ = ["MGP", "MGPStress", "MGPA", "MGPG", "MGP0"]
+__all__ = ["MGP", "MGPStress", "MGPA", "MGPG"]
 
 
 def MGPStress(rho, x=1.0, y=1.0, sigma=None, alpha=5.0 / 6.0, beta=5.0 / 6.0, calcType={"E", "V"}):
     pass
 
 
 @timer()
@@ -23,29 +23,29 @@
         beta=5.0 / 6.0,
         lumpfactor=0.2,
         maxpoint=1000,
         symmetrization=None,
         calcType={"E", "V"},
         split=False,
         ke_kernel_saved=None,
-        revke = True,
         **kwargs
 ):
     q = rho.grid.get_reciprocal().q
     rho0 = rho.amean()
     if ke_kernel_saved is None:
         KE_kernel_saved = {"Kernel": None, "rho0": 0.0, "shape": None}
     else:
         KE_kernel_saved = ke_kernel_saved
-    if abs(KE_kernel_saved['rho0']-rho0) > 1E-6 or np.shape(rho) != KE_kernel_saved['shape'] :
+    # if abs(KE_kernel_saved['rho0']-rho0) > 1E-6 or np.shape(rho) != KE_kernel_saved['shape'] :
+    if abs(KE_kernel_saved["rho0"] - rho0) > 1e-2 or np.shape(rho) != KE_kernel_saved["shape"]:
         sprint("Re-calculate KE_kernel", comm=rho.mp.comm, level=1)
         KE_kernel = MGPKernel(q, rho0, maxpoints=maxpoint, symmetrization=symmetrization)
         if lumpfactor is not None:
-            Ne = rho0 * rho.grid.volume
-            KE_kernel += MGPOmegaE(q, Ne, lumpfactor, revke = revke)
+            Ne = rho0 * rho.grid.Volume
+            KE_kernel += MGPOmegaE(q, Ne, lumpfactor)
         # -----------------------------------------------------------------------
         # rh0 = 0.03;lumpfactor = 0.0;q = np.linspace(1E-3, 8, 10000).reshape((1, 1, 1, -1))
         # mgp = MGPKernel(q,rho0,  maxpoints = maxpoint, symmetrization = None, KernelTable = None)
         # mgpa = MGPKernel(q,rho0, maxpoints = maxpoint, symmetrization = 'Arithmetic', KernelTable = None)
         # mgpg = MGPKernel(q,rho0, maxpoints = maxpoint, symmetrization = 'Geometric', KernelTable = None)
         # np.savetxt('mgp.dat', np.c_[q.ravel()/2.0, mgp.ravel(), mgpa.ravel(), mgpg.ravel()])
         # stop
@@ -96,24 +96,7 @@
         maxpoint=1000,
         symmetrization="Geometric",
         calcType={"E", "V"},
         split=False,
         **kwargs
 ):
     return MGP(rho, x, y, sigma, alpha, beta, lumpfactor, maxpoint, "Geometric", calcType, split, **kwargs)
-
-def MGP0(
-        rho,
-        x=1.0,
-        y=1.0,
-        sigma=None,
-        alpha=5.0 / 6.0,
-        beta=5.0 / 6.0,
-        lumpfactor=0.2,
-        maxpoint=1000,
-        symmetrization=None,
-        calcType={"E", "V"},
-        split=False,
-        revke = False,
-        **kwargs
-):
-    return MGP(rho, x, y, sigma, alpha, beta, lumpfactor, maxpoint, symmetrization, calcType, split, revke=False, **kwargs)
```

### Comparing `dftpy-2.0.0/src/dftpy/functional/kedf/sm.py` & `dftpy-2.0.0rc2/src/dftpy/functional/kedf/sm.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/kedf/tf.py` & `dftpy-2.0.0rc2/src/dftpy/functional/kedf/tf.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/kedf/vw.py` & `dftpy-2.0.0rc2/src/dftpy/functional/kedf/vw.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/kedf/wt.py` & `dftpy-2.0.0rc2/src/dftpy/functional/kedf/wt.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/nonadiabatic/__init__.py` & `dftpy-2.0.0rc2/src/dftpy/functional/nonadiabatic/__init__.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/nonadiabatic/jp.py` & `dftpy-2.0.0rc2/src/dftpy/functional/nonadiabatic/jp.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/nonadiabatic/wcdhc.py` & `dftpy-2.0.0rc2/src/dftpy/functional/nonadiabatic/wcdhc.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/pseudo/__init__.py` & `dftpy-2.0.0rc2/src/dftpy/functional/pseudo/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from abc import abstractmethod
 
 import numpy as np
 import scipy.special as sp
 from scipy.interpolate import splrep, splev
 import re
 
-from dftpy.ewald import CBspline, ewald
+from dftpy.ewald import CBspline
 from dftpy.field import ReciprocalField, DirectField
 from dftpy.functional.abstract_functional import AbstractFunctional
 from dftpy.functional.functional_output import FunctionalOutput
-from dftpy.grid import DirectGrid, RadialGrid
+from dftpy.grid import DirectGrid
 from dftpy.math_utils import quartic_interpolation
 from dftpy.mpi import sprint, SerialComm, MP
 from dftpy.time_data import timer
 
 from dftpy.functional.pseudo.psp import PSP
 from dftpy.functional.pseudo.recpot import RECPOT
 from dftpy.functional.pseudo.upf import UPF
@@ -42,15 +42,15 @@
         pass
 
     @abstractmethod
     def restart(self):
         pass
 
     @abstractmethod
-    def forces(self):
+    def force(self):
         pass
 
     @abstractmethod
     def stress(self):
         pass
 
     @property
@@ -72,15 +72,15 @@
 # Only touch this class if you know what you are doing
 class LocalPseudo(AbstractLocalPseudo):
     """
     LocalPseudo class handles local pseudo potentials.
     This is a template class and should never be touched.
     """
 
-    def __init__(self, grid=None, ions=None, PP_list=None, PME=True, readpp = None, comm = None, BsplineOrder = 10, **kwargs):
+    def __init__(self, grid=None, ions=None, PP_list=None, PME=True, readpp = None, comm = None, **kwargs):
 
         self.type = 'PSEUDO'
         self.name = 'PSEUDO'
 
         if comm is None:
             if grid is not None :
                 comm = grid.mp.comm
@@ -91,33 +91,24 @@
         if PP_list is not None:
             self.readpp = ReadPseudo(PP_list, comm=comm, **kwargs)
         elif readpp is not None :
             self.readpp = readpp
         else:
             raise AttributeError("Must specify PP_list for Pseudopotentials")
 
-        self.PME = PME
-        self.BsplineOrder = BsplineOrder
+        self.usePME = PME
         # if not PME :
             # sprint("Using N^2 method for strf!", comm=comm)
         self.restart(grid, ions)
 
     @property
     def _vloc_interp(self):
         return self.readpp.vloc_interp
 
     @property
-    def vloc_interp_core(self):
-        return self.readpp.vloc_interp_core
-
-    @property
-    def vloc_interp_atomic(self):
-        return self.readpp.vloc_interp_atomic
-
-    @property
     def _gp(self):
         return self.readpp.gp
 
     @property
     def _vp(self):
         return self.readpp.vp
 
@@ -125,54 +116,32 @@
     def PP_list(self):
         return self.readpp.PP_list
 
     @property
     def zval(self):
         return self.readpp.zval
 
-    @property
-    def core_density(self):
-        if self._core_density is None :
-            self._core_density = {}
-            reciprocal_grid = self.grid.get_reciprocal()
-            q = reciprocal_grid.q
-            v = np.zeros_like(q, dtype=np.complex128)
-            for key in sorted(self.vloc_interp_core):
-                for i in range(len(self.ions.positions)):
-                    if self.ions.symbols[i] == key:
-                        if self.vlines_core[key] is None : continue
-                        strf = self.ions.strf(reciprocal_grid, i)
-                        v += self.vlines_core[key] * strf
-            self._core_density = ReciprocalField(reciprocal_grid, griddata_3d=v).ifft(force_real=True)
-        return self._core_density
-
     def __repr__(self):
         return 'LOCALPSEUDO'
 
     def restart(self, grid=None, ions=None, full=False, duplicate=False):
         """
         Clean all private data and resets the ions and grid.
         This will prompt the computation of a new pseudo
         without recomputing the local pp on the atoms.
         """
         if duplicate :
             pseudo = self.__class__(grid = grid, ions = ions, readpp = self.readpp)
             return pseudo
 
         self._vlines = {}  # PP for each atomic species on 3D PW grid
-        self._vlines_core = {}  # Core density for each atomic species on 3D PW grid
-        self._vlines_atomic = {}  # Atomic density for each atomic species on 3D PW grid
         self._v = None  # PP for atom on 3D PW grid
         self._vreal = None  # PP for atom on 3D real space
         self._ions = None
         self._grid = None
-        self._core_density = None
-        #
-        self._Bspline = None
-        self.ewald = None
         if ions is not None:
             self.ions = ions
         if grid is not None:
             self.grid = grid
 
     @property
     def grid(self):
@@ -199,26 +168,14 @@
         for key in value.symbols_uniq :
             if key not in self.PP_list:
                 raise ValueError("There is no pseudopotential for {:4s} atom".format(key))
         self._ions = value
         # update zval in ions
         self._ions.set_charges(self.zval)
 
-    @property
-    def Bspline(self):
-        if self._Bspline is None :
-            self._Bspline = CBspline(ions=self.ions, grid=self.grid, order=self.BsplineOrder)
-        return self._Bspline
-
-    def get_ewald(self, PME = None):
-        if self.ewald is None :
-            if PME is None : PME = self.PME
-            self.ewald = ewald(ions=self.ions, grid = self.grid, PME=PME, Bspline = self.Bspline)
-        return self.ewald
-
     def compute(self, density, calcType={"E", "V"}, **kwargs):
         if self._vreal is None:
             self.local_PP()
         pot = self._vreal
         if 'E' in calcType:
             if density.rank > 1:
                 rho = np.sum(density, axis=0)
@@ -229,84 +186,51 @@
             ene = 0.0
 
         if density.rank > 1:
             pot = pot.tile((density.rank, 1, 1, 1))
         return FunctionalOutput(name="eN", energy=ene, potential=pot)
 
     @timer()
-    def local_PP(self):
+    def local_PP(self, BsplineOrder=10):
         """
         """
+        # if BsplineOrder is not 10:
+        # warnings.warn("BsplineOrder not 10. Do you know what you are doing?")
+        self.BsplineOrder = BsplineOrder
+
         if self._v is None:
-            if self.PME:
+            if self.usePME:
                 self._PP_Reciprocal_PME()
             else:
                 self._PP_Reciprocal()
         if self._vreal is None:
             self._vreal = self._v.ifft(force_real=True)
 
     def stress(self, rho, energy=None):
         if rho is None:
             raise AttributeError("Must specify rho")
         if not isinstance(rho, (DirectField)):
             raise TypeError("rho must be DirectField")
-        self.local_PP()
-        if self.PME:
+        if self.usePME:
             s = self._StressPME(rho, energy)
         else:
             s = self._Stress(rho, energy)
         return s
 
-    def forces(self, rho):
+    def force(self, rho):
         if rho is None:
             raise AttributeError("Must specify rho")
         if not isinstance(rho, (DirectField)):
             raise TypeError("rho must be DirectField")
-        self.local_PP()
-        if self.PME:
+        if self.usePME:
             f = self._ForcePME(rho)
         else:
             f = self._Force(rho)
         return f
 
-    def calc_force_cc(self, potential = None, rhod = None, ions = None):
-        """Calculate the correction forces
-
-        Parameters
-        ----------
-        potential : field
-            Potential in real space.
-        rhod :
-            density of each element in reciprocal space
-        """
-        #
-        if rhod is None : rhod = self.vlines_core
-        if ions is None : ions = self.ions
-        grid = potential.grid
-        #
-        reciprocal_grid = grid.get_reciprocal()
-        forces = np.zeros((ions.nat, 3))
-        mask = reciprocal_grid.mask
-        g = reciprocal_grid.g
-
-        if potential.rank == 2 : potential = 0.5*(potential[0]+potential[1])
-        potg = potential.fft()
-
-        for key in sorted(ions.zval):
-                rhocg = rhod[key]
-                if rhocg is None : continue
-                for i in range(ions.nat):
-                    if ions.symbols[i] == key:
-                        strf = ions.istrf(reciprocal_grid, i)
-                        den = (potg[mask] * rhocg[mask] * strf[mask]).imag
-                        for j in range(3):
-                            forces[i, j] = np.einsum("i, i->", g[j][mask], den)
-        forces *= 2.0 / grid.volume
-        return forces
-
     @property
     def vreal(self):
         """
         The vloc represented on the real space grid.
         """
         if self._vreal is not None:
             return self._vreal
@@ -325,71 +249,50 @@
 
     @property
     def vlines(self):
         """
         The vloc for each atom type represented on the reciprocal space grid.
         """
         if not self._vlines:
-            self._vlines = self.calc_vlines(self._gp, self._vp, self._vloc_interp)
+            reciprocal_grid = self.grid.get_reciprocal()
+            q = reciprocal_grid.q
+            vloc = np.empty_like(q)
+            for key in sorted(self._vloc_interp):
+                vloc_interp = self._vloc_interp[key]
+                vloc[:] = 0.0
+                mask = q < self._gp[key][-1]
+                qmask = q[mask]
+                if len(qmask)>0 :
+                    vloc[mask] = splev(qmask, vloc_interp, der=0)
+                # quartic interpolation for small q
+                # -----------------------------------------------------------------------
+                mask = q < self._gp[key][1]
+                vp = self._vp[key]
+                dp = vp[1] - vp[0]
+                f = [vp[2], vp[1], vp[0], vp[1], vp[2]]
+                dx = q[mask] / dp
+                vloc[mask] = quartic_interpolation(f, dx)
+                # -----------------------------------------------------------------------
+                self._vlines[key] = vloc.copy()
         return self._vlines
 
-    @property
-    def vlines_core(self):
-        if not self._vlines_core:
-            self._vlines_core = self.calc_vlines(self.readpp._core_density_grid, self.readpp._core_density,
-                    self.vloc_interp_core)
-        return self._vlines_core
-
-    @property
-    def vlines_atomic(self):
-        if not self._vlines_atomic:
-            self._vlines_atomic = self.calc_vlines(self.readpp._atomic_density_grid, self.readpp._atomic_density,
-                    self.vloc_interp_atomic)
-        return self._vlines_atomic
-
-    def calc_vlines(self, gps, vps, interps):
-        vlines = {}
-        reciprocal_grid = self.grid.get_reciprocal()
-        q = reciprocal_grid.q
-        vloc = np.empty_like(q)
-        for key in sorted(interps):
-            interp = interps[key]
-            if interp is None :
-                vlines[key] = None
-                continue
-            vloc[:] = 0.0
-            mask = q < gps[key][-1]
-            qmask = q[mask]
-            if len(qmask)>0 :
-                vloc[mask] = splev(qmask, interp, der=0)
-            # quartic interpolation for small q
-            # -----------------------------------------------------------------------
-            mask = q < gps[key][1]
-            vp = vps[key]
-            dp = vp[1] - vp[0]
-            f = [vp[2], vp[1], vp[0], vp[1], vp[2]]
-            dx = q[mask] / dp
-            vloc[mask] = quartic_interpolation(f, dx)
-            # -----------------------------------------------------------------------
-            vlines[key] = vloc.copy()
-        return vlines
-
     def _PP_Reciprocal(self):
         reciprocal_grid = self.grid.get_reciprocal()
         q = reciprocal_grid.q
         v = np.zeros_like(q, dtype=np.complex128)
         for key in sorted(self._vloc_interp):
             for i in range(len(self.ions.positions)):
                 if self.ions.symbols[i] == key:
                     strf = self.ions.strf(reciprocal_grid, i)
                     v += self.vlines[key] * strf
         self._v = ReciprocalField(reciprocal_grid, griddata_3d=v)
         return "PP successfully interpolated"
 
     def _PP_Reciprocal_PME(self):
+        self.Bspline = CBspline(ions=self.ions, grid=self.grid, order=self.BsplineOrder)
         reciprocal_grid = self.grid.get_reciprocal()
         q = reciprocal_grid.q
         v = np.zeros_like(q, dtype=np.complex128)
         QA = np.empty(self.grid.nr)
         scaled_postions=self.ions.get_scaled_positions()
         for key in sorted(self._vloc_interp):
             QA[:] = 0.0
@@ -583,22 +486,19 @@
     def __init__(self, PP_list=None, comm=None, parallel = True, **kwargs):
         self._gp = {}  # 1D PP grid g-space
         self._vp = {}  # PP on 1D PP grid
         self._r = {}  # 1D PP grid r-space
         self._v = {}  # PP on 1D PP grid r-space
         self._info = {}
         self._vloc_interp = {}  # Interpolates recpot PP
-        self._vloc_interp_core = {}  # Interpolates core density
-        self._vloc_interp_atomic = {}  # Interpolates atomic density
         self._core_density_grid = {}
         self._core_density = {}  # the radial core charge density for the non-linear core correction in g-space
         self._atomic_density_grid = {}
         self._atomic_density = {}  # the radial atomic charge density in g-space
         self._zval = {}
-        self._pp = {}
 
         self.PP_list = PP_list
         #-----------------------------------------------------------------------
         if comm is None: comm = SerialComm()
         self.comm = comm
         self.parallel = parallel and comm.size > 1
         #-----------------------------------------------------------------------
@@ -630,68 +530,74 @@
 
         Args:
             key: Atomic symbol
             k: The degree of the spline fit of splrep, should keep use 3.
         """
         vloc_interp = splrep(self._gp[key][1:], self._vp[key][1:], k=k)
         self._vloc_interp[key] = vloc_interp
-        if self._core_density[key] is not None :
-            self._vloc_interp_core[key] = splrep(self._core_density_grid[key][1:], self._core_density[key][1:], k=k)
-        else :
-            self._vloc_interp_core[key] = None
-
-        if self._atomic_density[key] is not None :
-            self._vloc_interp_atomic[key] = splrep(self._atomic_density_grid[key][1:], self._atomic_density[key][1:], k=k)
-        else :
-            self._vloc_interp_atomic[key] = None
-
-    @staticmethod
-    def _real2recip(r, v, zval=0, MaxPoints=10000, Gmax=30, Gmin=1E-4, gp=None, rcut=None, **kwargs):
-        if gp is None :
-            gp = np.logspace(np.log10(Gmin), np.log10(Gmax), num=MaxPoints)
-            gp[0] = 0.0
-        #
-        if rcut :
-            mk = r < rcut + 1E-6
-        else :
-            mk = slice(None)
-        #
-        vr = v*r + zval
-        #
-        vp = RadialGrid(r[mk], vr[mk], direct=True, vr=True, **kwargs).ft(gp)
-        vp[1:] -= 4.0 * np.pi * zval / (gp[1:] ** 2)
-        return gp, vp
 
     @staticmethod
-    def _real2recip_erf(r, v, zval=0, MaxPoints=10000, Gmax=30, Gmin=1E-4, gp=None, rcut=None, **kwargs):
-        if gp is None :
-            gp = np.logspace(np.log10(Gmin), np.log10(Gmax), num=MaxPoints)
-            gp[0] = 0.0
-        #
-        if rcut :
-            mk = r < rcut + 1E-6
-        else :
-            mk = slice(None)
-        #
-        vr = v*r + zval
+    def _real2recip(r, v, zval=0, MaxPoints=10000, Gmax=30, Gmin=1E-4, method='simpson', comm=None, mp=None):
+        if mp is None : mp = MP(comm = comm)
+        gp = np.logspace(np.log10(Gmin), np.log10(Gmax), num=MaxPoints)
+        gp[0] = 0.0
         vp = np.zeros_like(gp)
-        #
-        from scipy.integrate import simps as integrate
-        vp[0] = (4.0 * np.pi) * integrate((vr[mk]*r[mk]), r[mk])
-        #
-        vr = v*r + zval*sp.erf(r)
-        vp[1:] = RadialGrid(r[mk], vr[mk], direct=True, vr=True, **kwargs).ft(gp[1:])
-        vp[1:] -= 4.0 * np.pi * zval * np.exp(-gp[1:]**2/4.0) / (gp[1:] ** 2)
+        if method == 'simpson':
+            try:
+                # new version of scipy=1.6.0 change the name to simpson
+                from scipy.integrate import simpson
+            except Exception:
+                from scipy.integrate import simps as simpson
+            vr = (v * r + zval) * r
+
+            lb, ub = mp.split_number(len(gp))
+            if mp.is_root : lb = 1
+
+            for k in range(lb, ub):
+                y = sp.spherical_jn(0, gp[k] * r) * vr
+                vp[k] = (4.0 * np.pi) * simpson(y, r)
+
+            if mp.is_mpi : vp = mp.vsum(vp)
+
+            vp[0] = (4.0 * np.pi) * simpson(vr, r)
+        else:
+            dr = np.empty_like(r)
+            dr[1:] = r[1:] - r[:-1]
+            dr[0] = r[0]
+            vr = (v * r + zval) * r * dr
+
+            lb, ub = mp.split_number(len(gp))
+            if mp.is_root : lb = 1
+
+            for k in range(lb, ub):
+                vp[k] = (4.0 * np.pi) * np.sum(sp.spherical_jn(0, gp[k] * r) * vr)
+
+            vp = mp.vsum(vp)
+
+            vp[0] = (4.0 * np.pi) * np.sum(vr)
+        vp[1:] -= 4.0 * np.pi * zval / (gp[1:] ** 2)
         return gp, vp
 
     @staticmethod
-    def _recip2real(gp, vp, MaxPoints=1001, Rmax=10, r=None, **kwargs):
+    def _recip2real(gp, vp, MaxPoints=1001, Rmax=10, r=None, comm=None, mp=None):
+        if mp is None : mp = MP(comm = comm)
         if r is None:
             r = np.linspace(0, Rmax, MaxPoints)
-        v = RadialGrid(gp, vp, direct=False, **kwargs).ft(r)
+        v = np.zeros_like(r)
+        dg = np.empty_like(gp)
+        dg[1:] = gp[1:] - gp[:-1]
+        dg[0] = gp[0]
+        vr = vp * gp * gp * dg
+
+        lb, ub = mp.split_number(len(r))
+
+        for i in range(lb, ub):
+            v[i] = (0.5 / np.pi ** 2) * np.sum(sp.spherical_jn(0, r[i] * gp) * vr)
+
+        v = mp.vsum(v)
         return r, v
 
     @staticmethod
     def _vloc2rho(r, v, r2=None):
         if r2 is None: r2 = r
         tck = splrep(r, v)
         dv1 = splev(r2[1:], tck, der=1)
@@ -735,15 +641,16 @@
                     pp = engine(self.PP_list[key])
                 else :
                     pp = None
                 pp = self.comm.bcast(pp)
             else :
                 pp = engine(self.PP_list[key])
 
-        self._pp[key] = pp
+        self.pp = pp
+
         self._gp[key] = pp.radial_grid
         self._vp[key] = pp.local_potential
         self._zval[key] = pp.zval
         self._info[key] = pp.info
         self._core_density[key] = pp.core_density
         self._core_density_grid[key]= pp.core_density_grid
         self._atomic_density[key] = pp.atomic_density
@@ -757,34 +664,23 @@
             self._r[key] = self._gp[key]
             self._v[key] = self._vp[key]
             self._gp[key], self._vp[key] = self._real2recip(self._r[key], self._v[key], self._zval[key], comm=comm, **kwargs)
             if self._core_density[key] is not None :
                 self._core_density_grid[key], self._core_density[key] = self._real2recip(self._core_density_grid[key], self._core_density[key], 0, comm=comm, **kwargs)
             if self._atomic_density[key] is not None :
                 self._atomic_density_grid[key], self._atomic_density[key] = self._real2recip(self._atomic_density_grid[key], self._atomic_density[key], 0, comm=comm, **kwargs)
+        self._vloc_interp[key] = splrep(self._gp[key][1:], self._vp[key][1:], k=k)
 
     @property
     def vloc_interp(self):
         if not self._vloc_interp:
             raise AttributeError("Must init ReadPseudo")
         return self._vloc_interp
 
     @property
-    def vloc_interp_core(self):
-        if not self._vloc_interp_core:
-            raise AttributeError("Must init ReadPseudo")
-        return self._vloc_interp_core
-
-    @property
-    def vloc_interp_atomic(self):
-        if not self._vloc_interp_atomic:
-            raise AttributeError("Must init ReadPseudo")
-        return self._vloc_interp_atomic
-
-    @property
     def gp(self):
         if not self._gp:
             raise AttributeError("Must init ReadPseudo")
         return self._gp
 
     @property
     def vp(self):
@@ -796,24 +692,12 @@
     def zval(self):
         if not self._zval:
             raise AttributeError("Must init ReadPseudo")
         return self._zval
 
     @property
     def info(self):
-        if not self._info:
-            raise AttributeError("Must init ReadPseudo")
         return self._info
 
     @info.setter
     def info(self, value):
         self._info = value
-
-    @property
-    def pp(self):
-        if not self._pp:
-            raise AttributeError("Must init ReadPseudo")
-        return self._pp
-
-    @pp.setter
-    def pp(self, value):
-        self._pp = value
```

### Comparing `dftpy-2.0.0/src/dftpy/functional/pseudo/abstract_pseudo.py` & `dftpy-2.0.0rc2/src/dftpy/functional/pseudo/abstract_pseudo.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/pseudo/layer_pseudo.py` & `dftpy-2.0.0rc2/src/dftpy/functional/pseudo/layer_pseudo.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/pseudo/psp.py` & `dftpy-2.0.0rc2/src/dftpy/functional/pseudo/psp.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/pseudo/recpot.py` & `dftpy-2.0.0rc2/src/dftpy/functional/pseudo/recpot.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/pseudo/usp.py` & `dftpy-2.0.0rc2/src/dftpy/functional/pseudo/usp.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/pseudo/xml.py` & `dftpy-2.0.0rc2/src/dftpy/functional/pseudo/xml.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/functional/xc/semilocal_xc.py` & `dftpy-2.0.0rc2/src/dftpy/functional/semilocal_xc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,104 @@
 # Drivers for LibXC
 
 import numpy as np
+import copy
 import os
 import json
 
 from dftpy.field import DirectField
+from dftpy.functional.abstract_functional import AbstractFunctional
 from dftpy.functional.functional_output import FunctionalOutput
 from dftpy.time_data import timer
 
 
+class XC(AbstractFunctional):
+    def __init__(self, xc=None, core_density=None, libxc=None, name=None, **kwargs):
+        self.type = 'XC'
+        self.name = name or 'XC'
+        self.energy = None
+        xc = xc or name
+        self.options = kwargs
+        self.options['xc'] = xc
+        self._core_density = core_density
+        if libxc is False :
+            if xc and xc.lower() == 'lda' :
+                self.xcfun = LDA
+            else :
+                raise AttributeError("Default one only support 'LDA', others please try with pylibxc.")
+        else :
+            if isinstance(libxc, bool) : libxc = None
+            self.options['libxc'] = libxc
+            if CheckLibXC(False):
+                self.xcfun = LibXC
+            elif xc and xc.lower() == 'lda':
+                self.xcfun = LDA
+            else :
+                raise ModuleNotFoundError("Install pylibxc to use this functionality")
+
+    @property
+    def core_density(self):
+        return self._core_density
+
+    @core_density.setter
+    def core_density(self, value):
+        self._core_density = value
+
+    def compute(self, density, calcType={"E", "V"}, **kwargs):
+        options = copy.deepcopy(self.options)
+        options.update(kwargs)
+        core_density = self.core_density
+        if core_density is None:
+            new_density = density
+        elif density.rank == core_density.rank:
+            new_density = density + core_density
+        elif density.rank == 2 and core_density.rank == 1:
+            new_density = density.copy()
+            new_density[0] += 0.5 * core_density
+            new_density[1] += 0.5 * core_density
+
+        functional = self.xcfun(new_density, calcType=calcType, **options)
+        if 'E' in calcType : self.energy = functional.energy
+        return functional
+
+    def stress(self, density, **kwargs):
+        options = copy.deepcopy(self.options)
+        options.update(kwargs)
+        energy = self.energy
+        stress=XCStress(density, energy=energy, **options)
+        return stress
+
+
 def CheckLibXC(stop = True):
     import importlib.util
 
     islibxc = importlib.util.find_spec("pylibxc")
     found = islibxc is not None
     if not found and stop :
         raise ModuleNotFoundError("Install LibXC and pylibxc to use this functionality")
     return found
 
 
-def Get_LibXC_Input(density, do_sigma = False, do_tau = False, do_lapl = False,
-        sigma = None, lapl = None, tau = None, **kwargs):
+def Get_LibXC_Input(density, do_sigma=True):
     inp = {}
     if density.rank > 1:
         rhoT = density.reshape((2, -1)).T
         inp["rho"] = rhoT.ravel()
     else:
         inp["rho"] = density.ravel()
-    if do_sigma :
-        if sigma is None:
-            sigma = density.sigma("standard")
+    if do_sigma:
+        # sigma = density.sigma()
+        sigma = density.sigma("standard")
         if density.rank > 1:
             sigma = sigma.reshape((3, -1)).T
         inp["sigma"] = sigma.ravel()
-    if do_lapl :
-        if lapl is None:
-            lapl = density.laplacian(force_real = True, sigma = None)
-        inp["lapl"] = lapl.ravel()
-    if do_tau :
-        if tau is None :
-            raise ValueError("Please give 'tau' for MGGA functional.")
-        inp["tau"] = tau.ravel()
     return inp
 
 
-def Get_LibXC_Output(out, density, **kwargs):
+def Get_LibXC_Output(out, density):
     if not isinstance(out, (dict)):
         raise TypeError("LibXC output must be a dictionary")
 
     OutFunctional = FunctionalOutput(name="LibXC")
 
     rank_dict = {
         "vrho": 2,
@@ -169,57 +219,52 @@
         OutFunctional.energy = ene
         OutFunctional.energydensity = edens
 
     return OutFunctional
 
 
 @timer()
-def LibXC(density, libxc=None, calcType={"E", "V"}, sigma = None, lapl = None, tau = None, **kwargs):
+def LibXC(density, libxc=None, calcType={"E", "V"}, **kwargs):
     """
      Output:
         - out_functional: a functional evaluated with LibXC
      Input:
         - density: a DirectField (rank=1)
         - libxc: strings like "gga_k_lc94", "gga_x_pbe" and "gga_c_pbe"
     """
     if CheckLibXC():
         from pylibxc.functional import LibXCFunctional
 
     do_sigma = False
-    do_lapl = False
-    do_tau = False
     #-----------------------------------------------------------------------
     libxc = get_libxc_names(libxc = libxc, **kwargs)
     #-----------------------------------------------------------------------
+    for value in libxc :
+        if not isinstance(value, str):
+            raise AttributeError(
+                    "{} must be LibXC functionals. Check pylibxc.util.xc_available_functional_names()".format(value)
+                    )
+            if value.startswith('hyb') or value.startswith('mgga'):
+                raise AttributeError('Hybrid and Meta-GGA functionals have not been implemented yet')
+        if value.startswith('gga'):
+            do_sigma = True
 
     if not libxc:
         raise AttributeError("Please give a short name 'xc' or a list 'libxc'.")
 
     if not isinstance(density, (DirectField)):
         raise TypeError("Density should be a DirectField")
     if density.rank == 1:
         polarization = "unpolarized"
     elif density.rank == 2:
         polarization = "polarized"
     else:
         raise AttributeError("Only support nspin=1 or 2.")
 
-    for value in libxc :
-        func = LibXCFunctional(value, polarization)
-        if value.startswith('hyb'):
-            raise AttributeError('Hybrid and Meta-GGA functionals have not been implemented yet')
-        if value.startswith('gga'):
-            do_sigma = True
-        elif value.startswith('mgga'):
-            do_sigma = True
-            do_tau = True
-            if func._needs_laplacian: do_lapl = True
-
-    inp = Get_LibXC_Input(density, do_sigma=do_sigma, do_tau = do_tau, do_lapl = do_lapl,
-            sigma = sigma, lapl = lapl, tau = tau, **kwargs)
+    inp = Get_LibXC_Input(density, do_sigma=do_sigma)
     kargs = {'do_exc': False, 'do_vxc': False}
     if 'E' in calcType or 'D' in calcType:
         kargs.update({'do_exc': True})
     if 'V' in calcType:
         kargs.update({'do_vxc': True})
     if 'V2' in calcType:
         kargs.update({'do_fxc': True})
@@ -229,18 +274,18 @@
         kargs.update({'do_lxc': True})
 
     out_functional = None
     for value in libxc :
         func = LibXCFunctional(value, polarization)
         out = func.compute(inp, **kargs)
         if out_functional is not None :
-            out_functional += Get_LibXC_Output(out, density, **kwargs)
+            out_functional += Get_LibXC_Output(out, density)
             out_functional.name += "_" + value
         else:
-            out_functional = Get_LibXC_Output(out, density, **kwargs)
+            out_functional = Get_LibXC_Output(out, density)
             out_functional.name = value
     return out_functional
 
 
 def PBE(density, calcType={"E", "V"}):
     return LibXC(density=density, libxc = ["gga_x_pbe", "gga_c_pbe"], calcType=calcType)
 
@@ -499,10 +544,8 @@
 
     # compatible with older version
     libxc_old = [v for k, v in kwargs.items() if k in ["k_str", "x_str", "c_str"] and v is not None]
     if len(libxc_old)>0 :
         # print('libxc', libxc, libxc_old)
         # warnings.warn(FutureWarning("'*_str' are deprecated; please use 'libxc' or 'xc'"))
         libxc = libxc_old
-    if libxc :
-        libxc = [x.lower() for x in libxc]
     return libxc
```

### Comparing `dftpy-2.0.0/src/dftpy/functional/xc/xc.json` & `dftpy-2.0.0rc2/src/dftpy/functional/xc.json`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/grid.py` & `dftpy-2.0.0rc2/src/dftpy/grid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 import numpy as np
-from scipy.interpolate import splrep, splev
-import scipy.special as sp
 from ase.cell import Cell
-from dftpy.math_utils import spacing2ecut, ecut2nr
-from dftpy.mpi import MP
 
 class BaseGrid:
     """
     Object representing a grid (Cell (lattice) plus discretization)
     extends Cell
 
     Attributes
@@ -19,30 +15,29 @@
     dV : volume of a grid point
 
     Node:
     Virtual class, DirectGrid and ReciprocalGrid should be used in actual applications
 
     """
 
-    def __init__(self, lattice, nr = None, origin=np.array([0.0, 0.0, 0.0]), full=True, direct=True,
-                 cplx=False, mp=None, ecut = None, **kwargs):
+    def __init__(self, lattice, nr, origin=np.array([0.0, 0.0, 0.0]), full=False, direct=True,
+                 cplx=False, mp=None, **kwargs):
         if mp is None :
+            from dftpy.mpi import MP
             mp = MP()
         self._origin = np.asarray(origin)
         if not isinstance(lattice, Cell):
             cell=Cell(lattice)
         else:
             cell=lattice
         #
         self.cplx = cplx
         self._cell = cell
         self._direct = direct
         #
-        if nr is None : nr = ecut2nr(ecut=ecut, lattice=lattice, **kwargs)
-        #
         self._nrR = np.array(nr, dtype = np.int32)
         self._nnrR = np.prod(self._nrR)
         self._dV = np.abs(self.cell.volume) / self._nnrR
         self._nrG = self._nrR.copy()
         if not full :
             self._nrG[-1] = self._nrG[-1] // 2 + 1
         self._nnrG = np.prod(self._nrG)
@@ -50,15 +45,14 @@
         self._mp = mp
         if self.cplx :
             full = True
         self.local_slice(nr, direct = direct, full = full, cplx = cplx, **kwargs)
         self._nnr = np.prod(self._nr)
         # print('nr_local', self.mp.comm.rank, self._nr, direct, self.mp.comm.size, flush = True)
         self._full = full
-        self._ecut = ecut
 
     def __eq__(self, other: 'BaseGrid') -> bool:
         if np.allclose(self.lattice, other.lattice) and np.allclose(self.nrR, other.nrR):
             return True
         else :
             return False
 
@@ -245,62 +239,33 @@
     def free(self):
         self.mp.free()
 
     @property
     def lattice(self):
         return self.cell.array
 
-    @property
-    def ecut(self):
-        if self._ecut is None :
-            if hasattr(self, 'guess_ecut'):
-                ecut = self.guess_ecut()
-            elif hasattr(self, 'get_direct'):
-                ecut = self.get_direct().guess_ecut()
-            else :
-                ecut = None
-        else :
-            ecut = self._ecut
-        return ecut
-
-    @ecut.setter
-    def ecut(self, value):
-        self._ecut = value
-        if hasattr(self, 'Dgrid'):
-            self._qmask = None
-            if hasattr(self.Dgrid, '_ecut'):
-                self.Dgrid._ecut = value
-        elif hasattr(self, 'RPgrid'):
-            if hasattr(self.RPgrid, '_ecut'):
-                self.RPgrid._ecut = value
-                self.RPgrid._qmask = None
-
 
 class DirectGrid(BaseGrid):
     """
         Attributes:
         ----------
         All of BaseGrid and DirectCell
 
         r : cartesian coordinates of each grid point
 
         s : crystal coordinates of each grid point
     """
 
-    def __init__(self, lattice, nr = None, origin=np.array([0.0, 0.0, 0.0]), full=True, uppergrid=None, **kwargs):
+    def __init__(self, lattice, nr, origin=np.array([0.0, 0.0, 0.0]), full=True, uppergrid=None, **kwargs):
         """
         Parameters
         ----------
         lattice : array_like[3,3]
             matrix containing the direct lattice vectors (as its colums)
         """
-        self.init_options = locals()
-        for k in ['__class__', 'self', 'kwargs', 'uppergrid'] :
-            self.init_options.pop(k, None)
-        self.init_options.update(kwargs)
         super().__init__(lattice=lattice, nr=nr, origin=origin, full=full, direct=True, **kwargs)
         self._r = None
         self._rr = None
         self._s = None
         self.RPgrid = uppergrid
         self._Rtable = None
 
@@ -394,15 +359,15 @@
                 fac = 2 * np.pi
             fac = 2 * np.pi
             bg = fac * np.linalg.inv(self.lattice)
             bg = bg.T
             reciprocal_lat = np.einsum("ij,i->ij", bg, scale)
 
             self.RPgrid = ReciprocalGrid(lattice=reciprocal_lat, nr=self.nrR, full=self.full, uppergrid=self,
-                                         cplx=self.cplx, mp=self.mp, ecut = self.ecut)
+                                         cplx=self.cplx, mp=self.mp)
         return self.RPgrid
 
     def get_Rtable(self, rcut=10):
         '''Only support for serial'''
         if self._Rtable is None:
             self._Rtable = {}
             metric = np.dot(self.lattice, self.lattice.T)
@@ -442,52 +407,43 @@
         mask1 = np.logical_and(xyz[1] > -1, xyz[1] < nr[1])
         np.logical_and(mask, mask1, out=mask)
         np.logical_and(xyz[2] > -1, xyz[2] < nr[2], out=mask1)
         np.logical_and(mask, mask1, out=mask)
         # -----------------------------------------------------------------------
         return mask
 
-    def guess_ecut(self):
-        spacings2 = self.cell.cellpar()[:3] / (self._nrR - 1)
-        spacings = 0.5*(self.spacings + spacings2)
-        return spacing2ecut(spacings.max())
 
 class ReciprocalGrid(BaseGrid):
     """
         Attributes:
         ----------
         All of BaseGrid and DirectCell
 
         g : coordinates of each point in the reciprocal cell
 
         gg : square of each g vector
     """
 
-    def __init__(self, lattice, nr = None, origin=np.array([0.0, 0.0, 0.0]), full=True, uppergrid=None, **kwargs):
+    def __init__(self, lattice, nr, origin=np.array([0.0, 0.0, 0.0]), full=False, uppergrid=None, **kwargs):
         """
         Parameters
         ----------
         lattice : array_like[3,3]
             matrix containing the direct lattice vectors (as its colums)
         """
-        self.init_options = locals()
-        for k in ['__class__', 'self', 'kwargs', 'uppergrid'] :
-            self.init_options.pop(k, None)
-        self.init_options.update(kwargs)
         super().__init__(lattice=lattice, nr=nr, origin=origin, full=full, direct=False, **kwargs)
         self._g = None
         self._gg = None
         self.Dgrid = uppergrid
         self._q = None
         self._mask = None
         self._gF = None
         self._ggF = None
         self._invgg = None
         self._invq = None
-        self._gmask = None
 
     def __eq__(self, other):
         """
         Implement the == operator in the ReciprocalGrid class.
         Refer to the __eq__ method of Grid for more information.
         """
         if not isinstance(other, ReciprocalGrid):
@@ -562,15 +518,15 @@
             scale = np.array(scale)
             fac = 1.0
             if convention == "physics" or convention == "p":
                 fac = 1.0 / (2 * np.pi)
             at = np.linalg.inv(self.lattice.T * fac)
             direct_lat = np.einsum("ij,i->ij", at, 1.0 / scale)
             self.Dgrid = DirectGrid(lattice=direct_lat, nr=self.nrR, full=self.full, uppergrid=self, cplx=self.cplx,
-                                    mp=self.mp, ecut = self._ecut)
+                                    mp=self.mp)
         return self.Dgrid
 
     def _calc_grid_points(self, full=None):
         ax = []
         for i in range(3):
             # use fftfreq function so we don't have to
             # worry about odd or even number of points
@@ -616,14 +572,15 @@
             # mask = np.ones((nr[0], nr[1], Dnr[2]+1), dtype = bool)
             Dnr = nrR[:3] // 2
             Dmod = nrR[:3] % 2
             mask = np.ones(self.nr[:3], dtype=bool)
             if np.all(self.nr == self.nrR):
                 mask[:, :, Dnr[2] + 1 :] = False
 
+            mask[0, 0, 0] = False
             mask[0, Dnr[1] + 1 :, 0] = False
             mask[Dnr[0] + 1 :, :, 0] = False
             if Dmod[2] == 0:
                 mask[0, 0, Dnr[2]] = False
                 mask[0, Dnr[1] + 1 :, Dnr[2]] = False
                 mask[Dnr[0] + 1 :, :, Dnr[2]] = False
                 if Dmod[1] == 0:
@@ -649,14 +606,16 @@
             Dnr = nrR[:3] // 2 - self.offsets
             Dnr = np.where(Dnr > 0, Dnr, 0)
             Dmod = nrR[:3] % 2
             mask = np.ones(self.nr[:3], dtype=bool)
             if np.all(self.nrG == self.nrR):
                 mask[:, :, Dnr[2] + 1 :] = False
 
+            if np.all(self.offsets == 0):
+                mask[0, 0, 0] = False
             if self.offsets[0] == self.offsets[2] == 0 :
                 mask[0, Dnr[1] + 1 :, 0] = False
             if self.offsets[2] == 0 :
                 mask[Dnr[0] + 1 :, :, 0] = False
             if Dmod[2] == 0:
                 if self.offsets[0] == 0 :
                     if self.offsets[1] == 0 :
@@ -691,110 +650,7 @@
         if self._ggF is None:
             if self._gF is None:
                 self._gF = self._calc_grid_points(full=True)
             ggF = np.einsum("lijk,lijk->ijk", self._gF, self._gF)
             self._ggF = ggF
             # self._ggF = np.reshape(gg, (*self._gF.shape, 1))
         return self._ggF
-
-    @property
-    def full(self):
-        return self._full
-
-    @full.setter
-    def full(self, value):
-        if self._full != value :
-            self._full = value
-
-    @property
-    def g2max(self):
-        return 2.0*self.ecut
-
-    def get_gmask(self, g2max = None):
-        if g2max is None : return self.gmask
-        gmask = self.gg <= g2max
-        return gmask
-
-    @property
-    def gmask(self):
-        if self._gmask is None :
-            self._gmask = self.get_gmask(self.g2max)
-        return self._gmask
-
-
-class RadialGrid(object):
-    def __init__(self, r = None, v = None, direct = True, vr = None, **kwargs):
-        self._r = r
-        self._v = v
-        self._vr = vr
-        self._v_interp = None
-        self.direct = direct
-
-    @property
-    def r(self):
-        return self._r
-
-    @r.setter
-    def r(self, r):
-        self._r = r
-
-    @property
-    def v(self):
-        return self._v
-
-    @v.setter
-    def v(self, v):
-        self._v = v
-
-    @property
-    def vr(self):
-        return self._vr
-
-    @property
-    def v_interp(self):
-        if self._v_interp is None :
-            self._v_interp = splrep(self.r, self.v)
-        return self._v_interp
-
-    def to_3d_grid(self, dist, direct = None, out = None):
-        if out is None :
-            results = np.zeros_like(dist)
-        else :
-            results = out
-        mask = dist < self._r[-1]
-        if np.count_nonzero(mask) > 0 :
-            results[mask] = splev(dist[mask], self.v_interp, der=0, ext=1)
-        return results
-
-    def _ft(self, x, method='simpson', comm=None, mp=None, **kwargs):
-        v = self.v
-        r = self.r
-        if mp is None : mp = MP(comm = comm)
-        vp = np.zeros_like(x)
-
-        if method == 'simpson':
-            from scipy.integrate import simps as integrate
-        elif method == 'trapezoid':
-            from scipy.integrate import trapz as integrate
-
-        if self.vr :
-            vr = v * r
-        else :
-            vr = v * r * r
-
-        lb, ub = mp.split_number(len(x))
-
-        for k in range(lb, ub):
-            y = sp.spherical_jn(0, x[k] * r) * vr
-            vp[k] = integrate(y, r)
-
-        vp = mp.vsum(vp)
-
-        return vp
-
-    def ft(self, x, method='simpson', mp=None, **kwargs):
-        y = self._ft(x, method=method, mp=mp, **kwargs)
-        if self.direct :
-            y *= (4.0 * np.pi)
-        else :
-            y *= (0.5 / np.pi ** 2)
-        return y
```

### Comparing `dftpy-2.0.0/src/dftpy/interface.py` & `dftpy-2.0.0rc2/src/dftpy/interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import numpy as np
 import os
 from dftpy.mpi import sprint
-from dftpy.optimization import Optimization, OESCF
+from dftpy.optimization import Optimization
 from dftpy.functional import Functional
 from dftpy.functional.total_functional import TotalFunctional
 from dftpy.constants import LEN_CONV, ENERGY_CONV, STRESS_CONV
 from dftpy.formats.io import read_density, write, read
 from dftpy.ewald import ewald
 from dftpy.grid import DirectGrid
 from dftpy.field import DirectField
 from dftpy.math_utils import ecut2nr
 from dftpy.functional.functional_output import FunctionalOutput
+from dftpy.functional.semilocal_xc import XCStress
+from dftpy.functional.kedf import KEDFStress
+from dftpy.functional.hartree import HartreeFunctionalStress
 from dftpy.config.config import PrintConf, ReadConf
 from dftpy.inverter import Inverter
 from dftpy.properties import get_electrostatic_potential
 from dftpy.utils import field2distrib
 
 
 def ConfigParser(config, ions=None, rhoini=None, pseudo=None, grid=None, mp = None):
@@ -81,24 +84,15 @@
         PSEUDO.grid = grid
         PSEUDO.ions = ions
     kedf_config = config["KEDF"].copy()
     if kedf_config.get('temperature', None):
         kedf_config['temperature'] *= ENERGY_CONV['eV']['Hartree']
     if kedf_config.get('temperature0', None):
         kedf_config['temperature0'] *= ENERGY_CONV['eV']['Hartree']
-    if config['OPT']['algorithm'] == 'OESCF' :
-        KE = Functional(type="KEDF", name='vW')
-        if config["KEDF"]["kedf"].startswith('GGA') or config["KEDF"]["kedf"].startswith('MGGA'):
-            kedf_config['gga_remove_vw'] = True
-        kedf_config['y'] = 0.0
-        kedf_emb = Functional(type="KEDF", name=config["KEDF"]["kedf"], **kedf_config)
-        evaluator_emb = TotalFunctional(KEDF_EMB = kedf_emb)
-    else :
-        KE = Functional(type="KEDF", name=config["KEDF"]["kedf"], **kedf_config)
-        evaluator_emb = None
+    KE = Functional(type="KEDF", name=config["KEDF"]["kedf"], **kedf_config)
     ############################## XC and Hartree ##############################
     HARTREE = Functional(type="HARTREE")
     XC = Functional(type="XC", name=config["EXC"]["xc"], **config["EXC"])
     if config["NONADIABATIC"]["nonadiabatic"] is None:
         DYNAMIC = None
     else:
         DYNAMIC = Functional(type="DYNAMIC", name=config["NONADIABATIC"]["nonadiabatic"], **config["NONADIABATIC"])
@@ -131,47 +125,37 @@
         for ip in range(nspin):
             rho_ini[ip] += 1.0/nspin *(-1)**ip * magmom/ ions.cell.volume
     #-----------------------------------------------------------------------
     # The last is a dictionary, which return some properties are used for different situations.
     others = {
         "ions": ions,
         "field": rho_ini,
-        "rho": rho_ini,
         "E_v_Evaluator": E_v_Evaluator,
         "nr2": nr2,
-        "evaluator_emb" : evaluator_emb,
     }
     return config, others
 
 
-def OptimizeDensityConf(config, ions = None, rho = None, E_v_Evaluator = None, nr2 = None, evaluator_emb = None, **kwargs):
+def OptimizeDensityConf(config, ions, rho, E_v_Evaluator, nr2 = None):
     rho_ini = rho
     grid = rho_ini.grid
     if hasattr(E_v_Evaluator, 'PSEUDO'):
         PSEUDO=E_v_Evaluator.PSEUDO
     nr = grid.nr
     charge_total = ions.get_ncharges()
-    if config['OPT']['algorithm'] == 'OESCF' :
-        lscf = True
-    else :
-        lscf = False
     if "Optdensity" in config["JOB"]["task"]:
-        optimization_options = config["OPT"].copy()
+        optimization_options = config["OPT"]
         optimization_options["econv"] *= ions.nat
         # if config['MATH']['twostep'] :
         # optimization_options["econv"] *= 10
-        if lscf : optimization_options['algorithm'] = 'EMM'
         opt = Optimization(
             EnergyEvaluator=E_v_Evaluator,
             optimization_options=optimization_options,
             optimization_method=config["OPT"]["method"],
         )
-        if lscf :
-            oescf = OESCF(optimization = opt, evaluator_emb = evaluator_emb)
-            opt = oescf
         rho = opt.optimize_rho(guess_rho=rho_ini)
         # perform second step, dense grid
         # -----------------------------------------------------------------------
         for istep in range(2, config["MATH"]["multistep"] + 1):
             if istep == config["MATH"]["multistep"]:
                 if nr2 is None :
                     nr2 = nr * 2
@@ -181,73 +165,104 @@
             sprint("#" * 80)
             sprint("MULTI-STEP: Perform %d optimization step" % istep)
             sprint("Grid size of %d" % istep, " step is ", nr)
             grid2 = DirectGrid(lattice=grid.lattice, nr=nr, full=config["GRID"]["gfull"], mp=grid.mp)
             rho_ini = DirectField(grid=grid2, rank=rho.rank)
             field2distrib(rho, rho_ini, root = 0)
             rho_ini *= charge_total / (np.sum(rho_ini.integral()))
+            # ions.restart()
             if hasattr(E_v_Evaluator, 'PSEUDO'):
                 PSEUDO=E_v_Evaluator.PSEUDO
                 PSEUDO.restart(full=False, ions=PSEUDO.ions, grid=grid2)
+            opt = Optimization(
+                EnergyEvaluator=E_v_Evaluator,
+                optimization_options=optimization_options,
+                optimization_method=config["OPT"]["method"],
+            )
             rho = opt.optimize_rho(guess_rho=rho_ini)
         optimization_options["econv"] /= ions.nat  # reset the value
     ############################## calctype  ##############################
-    if lscf : E_v_Evaluator.UpdateFunctional(newFuncDict=evaluator_emb.funcDict)
+    linearii = config["MATH"]["linearii"]
+    linearie = config["MATH"]["linearie"]
+    energypotential = {}
     forces = {}
     stress = {}
     sprint("-" * 80)
-    calcType = set()
-    energypotential = {'TOTAL' : FunctionalOutput(name ='TOTAL', energy = 0.0)}
-
-    if 'Both' in config["JOB"]["calctype"]: calcType.update({"E", "V"})
-    if 'Potential' in config["JOB"]["calctype"]: calcType.update("V")
-    if 'Energy' in config["JOB"]["calctype"]: calcType.update("E")
-
-    if len(calcType) > 0 :
-        sprint("Calculate Energy/Potential...")
-        energypotential = E_v_Evaluator.get_energy_potential(rho, calcType=calcType, split = True)
-
-    if 'E' in calcType :
-        sprint(format("Energy information", "-^80"))
-        keys = list(energypotential.keys())
-        ke_energy = 0.0
-        for key in sorted(keys):
-            if key == "TOTAL":
-                continue
-            value = energypotential[key].energy
-            sprint("{:>10s} energy (eV): {:22.15E}".format(key, value * ENERGY_CONV["Hartree"]["eV"]))
-            if key.startswith('KEDF'): ke_energy += value
-        etot = energypotential["TOTAL"].energy
-        sprint("{:>10s} energy (eV): {:22.15E}".format("TOTAL", etot * ENERGY_CONV["Hartree"]["eV"]))
-        sprint("-" * 80)
+    if "Both" in config["JOB"]["calctype"]:
+        sprint("Calculate Energy and Potential...")
+        energypotential = GetEnergyPotential(
+            ions, rho, E_v_Evaluator, calcType=["E","V"], linearii=linearii, linearie=linearie
+        )
+    elif "Potential" in config["JOB"]["calctype"]:
+        sprint("Calculate Potential...")
+        energypotential = GetEnergyPotential(
+            ions, rho, E_v_Evaluator, calcType=["V"], linearii=linearii, linearie=linearie
+        )
+    elif "Density" in config["JOB"]["calctype"]:
+        sprint("Only return density...")
+        energypotential = {'TOTAL' : FunctionalOutput(name ='TOTAL', energy = 0.0)}
+    else:
+        sprint("Calculate Energy...")
+        energypotential = GetEnergyPotential(
+            ions, rho, E_v_Evaluator, calcType=["E"], linearii=linearii, linearie=linearie
+        )
+    sprint(format("Energy information", "-^80"))
+    keys, ep = zip(*energypotential.items())
+    values = [item.energy for item in ep]
+    values = rho.mp.vsum(values)
+    ep_w = dict(zip(keys, values))
+    ke_energy = 0.0
+    for key in sorted(keys):
+        if key == "TOTAL":
+            continue
+        value = ep_w[key]
+        sprint("{:>10s} energy (eV): {:22.15E}".format(key, ep_w[key]* ENERGY_CONV["Hartree"]["eV"]))
+        if key.startswith('KEDF'): ke_energy += ep_w[key]
+    etot = ep_w['TOTAL']
+    sprint("{:>10s} energy (eV): {:22.15E}".format("TOTAL", etot * ENERGY_CONV["Hartree"]["eV"]))
+    sprint("-" * 80)
 
-        etot_eV = etot * ENERGY_CONV["Hartree"]["eV"]
-        etot_eV_patom = etot * ENERGY_CONV["Hartree"]["eV"] / ions.nat
-        fstr = "  {:<30s} : {:30.15f}"
-        sprint(fstr.format("kedfs energy (a.u.)", ke_energy))
-        sprint(fstr.format("kedfs energy (eV)", ke_energy* ENERGY_CONV["Hartree"]["eV"]))
-        sprint(fstr.format("total energy (a.u.)", etot))
-        sprint(fstr.format("total energy (eV)", etot_eV))
-        sprint(fstr.format("total energy (eV/atom)", etot_eV_patom))
+    etot_eV = etot * ENERGY_CONV["Hartree"]["eV"]
+    etot_eV_patom = etot * ENERGY_CONV["Hartree"]["eV"] / ions.nat
+    fstr = "  {:<30s} : {:30.15f}"
+    sprint(fstr.format("kedfs energy (a.u.)", ke_energy))
+    sprint(fstr.format("kedfs energy (eV)", ke_energy* ENERGY_CONV["Hartree"]["eV"]))
+    sprint(fstr.format("total energy (a.u.)", etot))
+    sprint(fstr.format("total energy (eV)", etot_eV))
+    sprint(fstr.format("total energy (eV/atom)", etot_eV_patom))
     ############################## Force ##############################
     if "Force" in config["JOB"]["calctype"]:
         sprint("Calculate Force...")
-        forces = E_v_Evaluator.get_forces(rho, ions = ions, split = True)
+        forces = GetForces(ions, rho, E_v_Evaluator, linearii=linearii, linearie=linearie, PPlist=None)
         ############################## Output Force ##############################
         f = np.abs(forces["TOTAL"])
         fmax, fmin, fave = np.max(f), np.min(f), np.mean(f)
         fstr_f = " " * 8 + "{0:>22s} : {1:<22.5f}"
         sprint(fstr_f.format("Max force (a.u.)", fmax))
         sprint(fstr_f.format("Min force (a.u.)", fmin))
         sprint(fstr_f.format("Ave force (a.u.)", fave))
+        # fstr_f =' ' * 16 + '{0:<22s}{1:<22s}{2:<22s}'
+        # sprint(fstr_f.format('Max (a.u.)', 'Min (a.u.)', 'Ave (a.u.)'))
+        # fstr_f =' ' * 16 + '{0:<22.5f} {1:<22.5f} {2:<22.5f}'
+        # sprint(fstr_f.format(fmax, fmin, fave))
         sprint("-" * 80)
     ############################## Stress ##############################
     if "Stress" in config["JOB"]["calctype"]:
         sprint("Calculate Stress...")
-        stress = E_v_Evaluator.get_stress(rho, split=True)
+        stress = GetStress(
+            ions,
+            rho,
+            E_v_Evaluator,
+            energypotential=energypotential,
+            xc_options=config["EXC"],
+            ke_options=config["KEDF"],
+            linearii=linearii,
+            linearie=linearie,
+            PPlist=None,
+        )
         ############################## Output stress ##############################
         fstr_s = " " * 16 + "{0[0]:12.5f} {0[1]:12.5f} {0[2]:12.5f}"
         if config["OUTPUT"]["stress"]:
             for key in sorted(stress.keys()):
                 if key == "TOTAL":
                     continue
                 value = stress[key]
@@ -275,26 +290,180 @@
     results = {}
     results["density"] = rho
     results["energypotential"] = energypotential
     results["forces"] = forces
     results["stress"] = stress
     if hasattr(E_v_Evaluator, 'PSEUDO'):
         results["pseudo"] = PSEUDO
-    if lscf : E_v_Evaluator.UpdateFunctional(keysToRemove=evaluator_emb.funcDict)
     # sprint('-' * 31, 'Time information', '-' * 31)
     # -----------------------------------------------------------------------
     return results
 
 
+def GetEnergyPotential(ions, rho, EnergyEvaluator, calcType={"E","V"}, linearii=True, linearie=True):
+    energypotential = {}
+    ewaldobj = ewald(rho=rho, ions=ions, PME=linearii)
+    energypotential["II"] = FunctionalOutput(name="Ewald", potential=np.zeros_like(rho), energy=ewaldobj.energy)
+
+    energypotential["TOTAL"] = energypotential["II"].copy()
+    funcDict = EnergyEvaluator.funcDict
+    for key, func in funcDict.items():
+        if func.type == "KEDF":
+            results = func(rho, calcType=calcType, split=True)
+            for key2 in results:
+                energypotential["TOTAL"] += results[key2]
+                energypotential["KEDF-" + key2.split('-')[-1]] = results[key2]
+        else :
+            results = func(rho, calcType=calcType)
+            energypotential["TOTAL"] += results
+            energypotential[func.type] = results
+
+    # keys, ep = zip(*energypotential.items())
+    # values = [item.energy for item in ep]
+    # values = mp.vsum(values)
+    # for item, v in zip(ep, values):
+        # item.energy = v
+    return energypotential
+
+
+def GetForces(ions, rho, EnergyEvaluator, linearii=True, linearie=True, PPlist=None):
+    forces = {}
+    forces["PSEUDO"] = EnergyEvaluator.PSEUDO.force(rho)
+    ewaldobj = ewald(rho=rho, ions=ions, verbose=False, PME=linearii)
+    forces["II"] = ewaldobj.forces
+    forces["TOTAL"] = forces["PSEUDO"] + forces["II"]
+    forces["TOTAL"] = rho.mp.vsum(forces["TOTAL"])
+    return forces
+
+
+def GetStress_old(
+    ions,
+    rho,
+    EnergyEvaluator,
+    energypotential=None,
+    energy=None,
+    xc_options = {'xc' : 'LDA'},
+    ke_options={"kedf" : "WT", "x": 1.0, "y": 1.0},
+    linearii=True,
+    linearie=True,
+    PPlist=None,
+):
+    """
+    Get stress tensor
+    """
+    #-----------------------------------------------------------------------
+    KEDF_Stress_L= {
+            "TF" : ["TF"],
+            "VW": ["VW"],
+            "X_TF_Y_VW": ["TF", "VW"],
+            "TFVW": ["TF", "VW"],
+            "WT": ["TF", "VW", "NL"],
+            }
+    ke = ke_options["kedf"]
+    if ke not in KEDF_Stress_L :
+        raise AttributeError("%s KEDF have not implemented for stress" % ke)
+    kelist = KEDF_Stress_L[ke]
+    #-----------------------------------------------------------------------
+    #Initial energy dict
+    energy = {}
+    if energypotential is not None:
+        for key in energypotential :
+            energy[key] = energypotential[key].energy
+    elif energy is None :
+        funcDict = EnergyEvaluator.funcDict
+        for key in funcDict :
+            func = getattr(EnergyEvaluator, key)
+            if func.type.startwith('KEDF'):
+                for item in kelist :
+                    energy['KEDF-' + item] = None
+            else :
+                energy[func.type] = None
+
+    stress = {}
+    stress['TOTAL'] = np.zeros((3, 3))
+
+    for key1 in energy :
+        if key1 == "TOTAL" :
+            continue
+        elif key1 == "II" :
+            ewaldobj = ewald(rho=rho, ions=ions, verbose=False, PME=linearii)
+            stress[key1] = ewaldobj.stress
+        elif key1 == "XC" :
+            stress[key1] = XCStress(rho, energy=energy[key1], **xc_options)
+        elif key1 == 'HARTREE' :
+            stress[key1] = HartreeFunctionalStress(rho, energy=energy[key1])
+        elif key1 == 'PSEUDO' :
+            stress[key1] = EnergyEvaluator.PSEUDO.stress(rho, energy=energy[key1])
+        elif key1.startswith('KEDF') :
+            if "TF" in key1 :
+                stress[key1] = KEDFStress(rho, name="TF", energy=energy[key1], **ke_options)
+            if "VW" in key1 :
+                stress[key1] = KEDFStress(rho, name="VW", energy=energy[key1], **ke_options)
+            if 'NL' in key1 :
+                stress[key1] = KEDFStress(rho, name=ke, energy=energy[key1], **ke_options)
+        else :
+            raise AttributeError("%s have not implemented for stress" % key1)
+        stress['TOTAL'] += stress[key1]
+
+    for i in range(1, 3):
+        for j in range(i - 1, -1, -1):
+            stress["TOTAL"][i, j] = stress["TOTAL"][j, i]
+
+    keys, values = zip(*stress.items())
+    values = rho.mp.vsum(values)
+    stress = dict(zip(keys, values))
+
+    return stress
+
 def InvertRunner(config, ions, EnergyEvaluater):
     file_rho_in = config["INVERSION"]["rho_in"]
     file_v_out = config["INVERSION"]["v_out"]
     field = read_density(file_rho_in)
 
     if ions.cell != field.cell :
         raise ValueError('The grid of the input density does not match the grid of the system')
 
     inv = Inverter()
     ext = inv(field, EnergyEvaluater)
     write(file_v_out, data=ext.v, ions=ions, data_type='potential')
 
     return ext
+
+def GetStress(
+    ions,
+    rho,
+    EnergyEvaluator,
+    linearii=True,
+    ewaldobj= None,
+    **kwargs
+):
+    """
+    Get stress tensor
+    """
+    #-----------------------------------------------------------------------
+    stress = {}
+    if ewaldobj is None :
+        ewaldobj = ewald(rho=rho, ions=ions, verbose=False, PME=linearii)
+    stress['II'] = ewaldobj.stress
+    stress['TOTAL'] = stress['II'].copy()
+
+    funcDict = EnergyEvaluator.funcDict
+    for key, func in funcDict.items():
+        if func.type == "KEDF":
+            results = func.stress(rho, split=True)
+            for key2 in results:
+                stress["TOTAL"] += results[key2]
+                stress["KEDF-" + key2.split('-')[-1]] = results[key2]
+        else :
+            results = func.stress(rho)
+            stress["TOTAL"] += results
+            stress[func.type] = results
+
+    for i in range(1, 3):
+        for j in range(i - 1, -1, -1):
+            stress["TOTAL"][i, j] = stress["TOTAL"][j, i]
+
+    keys, values = zip(*stress.items())
+    values = rho.mp.vsum(values)
+    stress = dict(zip(keys, values))
+
+    return stress
```

### Comparing `dftpy-2.0.0/src/dftpy/inverter.py` & `dftpy-2.0.0rc2/src/dftpy/inverter.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/ions.py` & `dftpy-2.0.0rc2/src/dftpy/ions.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,14 @@
             celldisp=None,
             constraint=None,
             calculator=None,
             info=None,
             velocities=None,
             units = 'au'):
 
-        self.init_options = locals()
-        for k in ['__class__', 'self'] :
-            self.init_options.pop(k, None)
-
         super().__init__(
             symbols=symbols,
             positions=positions,
             numbers=numbers,
             tags=tags,
             momenta=momenta,
             masses=masses,
```

### Comparing `dftpy-2.0.0/src/dftpy/linear_solver.py` & `dftpy-2.0.0rc2/src/dftpy/linear_solver.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/math_utils.py` & `dftpy-2.0.0rc2/src/dftpy/math_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -394,26 +394,28 @@
     https ://en.wikipedia.org/wiki/Conjugate_gradient_method
     HS->DY->CD
 
     """
     asum = resA[-1].grid.mp.asum if hasattr(resA[-1], 'grid') else np.sum
     if len(resA) == 1:
         beta = 0.0
-    elif method in ["CG-HS", "CG"] and len(dirA) > 0:  # Works better than others in most tests
+    elif method == "CG-HS" and len(dirA) > 0:  # Maybe the best of the CG.
         beta = asum(resA[-1] * (resA[-1] - resA[-2])) / asum(dirA[-1] * (resA[-1] - resA[-2]))
+    elif method == "CG-FR":
+        beta = asum(resA[-1] ** 2) / asum(resA[-2] ** 2)
     elif method == "CG-PR":
         beta = asum(resA[-1] * (resA[-1] - resA[-2])) / asum(resA[-2] ** 2)
         beta = max(beta, 0.0)
     elif method == "CG-DY" and len(dirA) > 0:
         beta = asum(resA[-1] ** 2) / asum(dirA[-1] * (resA[-1] - resA[-2]))
     elif method == "CG-CD" and len(dirA) > 0:
         beta = -(resA[-1] ** 2) / asum(dirA[-1] * resA[-2])
     elif method == "CG-LS" and len(dirA) > 0:
         beta = asum(resA[-1] * (resA[-1] - resA[-2])) / asum(dirA[-1] * resA[-2])
-    else: # CG-FR or regular CG
+    else:
         beta = asum(resA[-1] ** 2) / asum(resA[-2] ** 2)
 
     if dirA is None or len(dirA) == 0:
         direction = -resA[-1]
     else:
         direction = -resA[-1] + beta * dirA[-1]
 
@@ -458,31 +460,7 @@
         t2 = -f[0] + 16.0 * f[1] - 30.0 * f[2] + 16.0 * f[3] - f[4]
         t3 = -2.0 * f[0] + 4.0 * f[1] - 4.0 * f[3] + 2.0 * f[4]
         t4 = f[0] - 4.0 * f[1] + 6.0 * f[2] - 4.0 * f[3] + f[4]
         results = t0 + dx * (t1 + dx * (t2 + dx * (t3 + dx * t4)))/24.0
     else :
         raise AttributeError("Error : Not implemented yet")
     return results
-
-
-def gaussian(x, sigma = 0.1, mu = 0.0, dim = 3, deriv = 0):
-    y = 1.0/(np.sqrt(2.0 * np.pi) * sigma) ** dim * np.exp(-0.5 * ((x - mu)/sigma) ** 2.0)
-    if deriv == 0 :
-        pass
-    elif deriv == 1 :
-        y *= (mu-x)/sigma**2
-    else :
-        raise AttributeError(f"Sorry, the gaussian not support 'deriv' with {deriv}")
-    return y
-
-def gaussian_g(x, sigma = 0.1, dim = 3):
-    y = (np.sqrt(2.0 * np.pi) * sigma) ** (dim - 1) * np.exp(-0.5 * (x * sigma) ** 2)
-    return y
-
-def fermi_dirac(x, mu = None, kt = None):
-    if mu is None :
-        mu = 2.0/3.0 * np.max(x)
-    if kt is None :
-        kt = mu * 0.1
-    f = np.exp((x - mu)/kt) + 1.0
-    f = 1.0/f
-    return f
```

### Comparing `dftpy-2.0.0/src/dftpy/mpi/mp_mpi4py.py` & `dftpy-2.0.0rc2/src/dftpy/mpi/mp_mpi4py.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,27 +30,26 @@
             results = self.arr
             value[:] = input_array
             # results = self.fft.backward(value, results, normalize=False)
             results = self.fft.backward(value, results, normalize=True)
         return results
 
 
-def get_mpi4py_fft(comm, nr, decomposition = 'Slab', backend = None, grid = None, max_saved = 10, cplx = False, full = False, **kwargs):
+def get_mpi4py_fft(comm, nr, decomposition = 'Slab', backend = None, grid = None, max_saved = 10, cplx = False, **kwargs):
     """
     Note :
         'max_saved' means the number of fft objects saved. It should be manual release. see MP.free()
     """
     fft_support = ['pyfftw', 'numpy','scipy', 'mkl_fft']
     # fft_support = ['fftw', 'pyfftw', 'numpy','scipy', 'mkl_fft']
     if backend not in fft_support :
         backend = environ["FFTLIB"]
     if backend not in fft_support :
         backend = 'numpy'
 
-    cplx = cplx or full
     if cplx :
         backend = 'numpy' # If cplx, use numpy for safe
         dtype = np.complex
     else :
         dtype = np.float
 
     global fft_saved
```

### Comparing `dftpy-2.0.0/src/dftpy/mpi/mp_serial.py` & `dftpy-2.0.0rc2/src/dftpy/mpi/mp_serial.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/mpi/mpi.py` & `dftpy-2.0.0rc2/src/dftpy/mpi/mpi.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/mpi/utils.py` & `dftpy-2.0.0rc2/src/dftpy/mpi/utils.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/optimization/optimization.py` & `dftpy-2.0.0rc2/src/dftpy/optimization.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/optimize.py` & `dftpy-2.0.0rc2/src/dftpy/optimize.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/td/casida.py` & `dftpy-2.0.0rc2/src/dftpy/td/casida.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/td/hamiltonian.py` & `dftpy-2.0.0rc2/src/dftpy/td/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/td/interface.py` & `dftpy-2.0.0rc2/src/dftpy/td/interface.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/td/operator.py` & `dftpy-2.0.0rc2/src/dftpy/td/operator.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/td/predictor_corrector.py` & `dftpy-2.0.0rc2/src/dftpy/td/predictor_corrector.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/td/propagator/__init__.py` & `dftpy-2.0.0rc2/src/dftpy/td/propagator/__init__.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/td/propagator/abstract_propagator.py` & `dftpy-2.0.0rc2/src/dftpy/td/propagator/abstract_propagator.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/td/propagator/crank_nicholson.py` & `dftpy-2.0.0rc2/src/dftpy/td/propagator/crank_nicholson.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/td/propagator/taylor.py` & `dftpy-2.0.0rc2/src/dftpy/td/propagator/taylor.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/td/real_time_runner.py` & `dftpy-2.0.0rc2/src/dftpy/td/real_time_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,17 +72,17 @@
         self.z_split = config["TD"]['z_split'] / Units.Bohr
 
         if self.vector_potential:
             self.A_t = None
             self.A_tm1 = None
             self.Omega = config["TD"]["omega"]
             if self.Omega <= 0:
-                self.Omega = self.rho0.grid.volume
+                self.Omega = self.rho0.grid.Volume
             else:
-                self.Omega = self.rho0.grid.volume * self.Omega
+                self.Omega = self.rho0.grid.Volume * self.Omega
 
         if self.correction:
             correct_potential_dict = dict()
             if config['KEDF2']['active']:
                 correct_kedf = Functional(type='KEDF', name=config['KEDF2']['kedf'], **config['KEDF2'])
                 correct_potential_dict.update({'Nonlocal': correct_kedf})
             if config['NONADIABATIC2']['active']:
```

### Comparing `dftpy-2.0.0/src/dftpy/td/utils.py` & `dftpy-2.0.0rc2/src/dftpy/td/utils.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/time_data.py` & `dftpy-2.0.0rc2/src/dftpy/time_data.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/utils/__init__.py` & `dftpy-2.0.0rc2/src/dftpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/utils/utils.py` & `dftpy-2.0.0rc2/src/dftpy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/visualize/__init__.py` & `dftpy-2.0.0rc2/src/dftpy/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/visualize/ipv_viewer.py` & `dftpy-2.0.0rc2/src/dftpy/visualize/ipv_viewer.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/visualize/jupyter.py` & `dftpy-2.0.0rc2/src/dftpy/visualize/jupyter.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/visualize/mpl_viewer.py` & `dftpy-2.0.0rc2/src/dftpy/visualize/mpl_viewer.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy/visualize/vesta_viewer.py` & `dftpy-2.0.0rc2/src/dftpy/visualize/vesta_viewer.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.0/src/dftpy.egg-info/PKG-INFO` & `dftpy-2.0.0rc2/src/dftpy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: dftpy
-Version: 2.0.0
+Version: 2.0.0rc2
 Summary: Python3 packages for Density Functional Theory
 Home-page: http://dftpy.rutgers.edu
 Author: Pavanello Research Group
 Author-email: m.pavanello@rutgers.edu
 License: MIT
+Description: # DFTpy's Manual and Tutorials
+        
+        See [DFTpy's website](http://dftpy.rutgers.edu) for details.
+        
+        
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
+Provides-Extra: all
 Provides-Extra: libxc
-Provides-Extra: upf
 Provides-Extra: mpi
-Provides-Extra: all
-License-File: LICENSE.txt
-
-# DFTpy's Manual and Tutorials
-
-See [DFTpy's website](http://dftpy.rutgers.edu) for details.
-
-
-
-
+Provides-Extra: upf
```

### Comparing `dftpy-2.0.0/src/dftpy.egg-info/SOURCES.txt` & `dftpy-2.0.0rc2/src/dftpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -53,16 +53,14 @@
 examples/DATA/Mg_cluster.vasp
 examples/DATA/Mg_lda.oe01.recpot
 examples/DATA/al.gga.recpot
 examples/DATA/al.lda.lps
 examples/DATA/al.lda.psp
 examples/DATA/al.lda.recpot
 examples/DATA/al.lda.upf
-examples/DATA/al_random.in
-examples/DATA/al_random.xsf
 examples/DATA/as.lda.recpot
 examples/DATA/ase_opt.traj
 examples/DATA/cd.vasp
 examples/DATA/fcc.vasp
 examples/DATA/ga.lda.recpot
 examples/DATA/hd.vasp
 examples/DATA/in.lda.recpot
@@ -70,16 +68,14 @@
 examples/DATA/li.lda.recpot
 examples/DATA/md.traj
 examples/DATA/mg.lda.recpot
 examples/DATA/p.lda.recpot
 examples/DATA/sb.lda.recpot
 examples/DATA/si.gga.recpot
 examples/DATA/si.lda.recpot
-examples/DATA/ti.xsf
-examples/DATA/ti_pbe_v1.4.uspp.F.UPF
 examples/md/test_ase_npt.py
 examples/md/test_ase_nvt.py
 examples/md/test_ase_nvt_nh.py
 examples/md/traj2xyz.py
 examples/notebooks/density_optimization.ipynb
 examples/notebooks/td-ofdft-tutorial.ipynb
 examples/ofdft/config.ini
@@ -105,17 +101,15 @@
 examples/test/test_functional_LibXC.py
 examples/test/test_grid.py
 examples/test/test_linear_solver.py
 examples/test/test_mpi_grid.py
 examples/test/test_pme.py
 examples/test/test_propagator.py
 examples/test/test_read_pp.py
-examples/test/test_rvv10.py
 examples/test/test_snpy.py
-examples/test/test_xc.py
 scripts/convertPP.py
 scripts/convert_den.py
 scripts/convert_td.py
 scripts/dftpy
 scripts/invert
 scripts/opt_layer_pseudo.py
 scripts/quadrupole.py
@@ -129,14 +123,16 @@
 src/dftpy/field.py
 src/dftpy/grid.py
 src/dftpy/interface.py
 src/dftpy/inverter.py
 src/dftpy/ions.py
 src/dftpy/linear_solver.py
 src/dftpy/math_utils.py
+src/dftpy/mixer.py
+src/dftpy/optimization.py
 src/dftpy/optimize.py
 src/dftpy/time_data.py
 src/dftpy.egg-info/PKG-INFO
 src/dftpy.egg-info/SOURCES.txt
 src/dftpy.egg-info/dependency_links.txt
 src/dftpy.egg-info/requires.txt
 src/dftpy.egg-info/top_level.txt
@@ -145,15 +141,14 @@
 src/dftpy/api/dftd4.py
 src/dftpy/config/__init__.py
 src/dftpy/config/config.py
 src/dftpy/config/config_entry.py
 src/dftpy/config/configentries.json
 src/dftpy/cui/__init__.py
 src/dftpy/cui/main.py
-src/dftpy/density/__init__.py
 src/dftpy/density/density.py
 src/dftpy/formats/__init__.py
 src/dftpy/formats/ase_io.py
 src/dftpy/formats/cube.py
 src/dftpy/formats/den.py
 src/dftpy/formats/io.py
 src/dftpy/formats/npy.py
@@ -166,14 +161,15 @@
 src/dftpy/functional/__init__.py
 src/dftpy/functional/abstract_functional.py
 src/dftpy/functional/external_potential.py
 src/dftpy/functional/functional_output.py
 src/dftpy/functional/hartree.py
 src/dftpy/functional/semilocal_xc.py
 src/dftpy/functional/total_functional.py
+src/dftpy/functional/xc.json
 src/dftpy/functional/kedf/__init__.py
 src/dftpy/functional/kedf/fp.py
 src/dftpy/functional/kedf/gga.py
 src/dftpy/functional/kedf/hc.py
 src/dftpy/functional/kedf/kernel.py
 src/dftpy/functional/kedf/lkt.py
 src/dftpy/functional/kedf/lwt.py
@@ -189,32 +185,24 @@
 src/dftpy/functional/pseudo/abstract_pseudo.py
 src/dftpy/functional/pseudo/layer_pseudo.py
 src/dftpy/functional/pseudo/psp.py
 src/dftpy/functional/pseudo/recpot.py
 src/dftpy/functional/pseudo/upf.py
 src/dftpy/functional/pseudo/usp.py
 src/dftpy/functional/pseudo/xml.py
-src/dftpy/functional/xc/__init__.py
-src/dftpy/functional/xc/rvv10.py
-src/dftpy/functional/xc/semilocal_xc.py
-src/dftpy/functional/xc/xc.json
-src/dftpy/invert/__init__.py
-src/dftpy/invert/analysis.py
-src/dftpy/mixer/__init__.py
-src/dftpy/mixer/linear.py
-src/dftpy/mixer/mixer.py
-src/dftpy/mixer/pulay.py
 src/dftpy/mpi/__init__.py
 src/dftpy/mpi/mp_mpi4py.py
 src/dftpy/mpi/mp_serial.py
 src/dftpy/mpi/mpi.py
 src/dftpy/mpi/utils.py
-src/dftpy/optimization/__init__.py
-src/dftpy/optimization/optimization.py
-src/dftpy/optimization/scf.py
+src/dftpy/old/atom.py
+src/dftpy/old/cell.py
+src/dftpy/old/coord.py
+src/dftpy/old/pbc_array.py
+src/dftpy/old/system.py
 src/dftpy/properties/__init__.py
 src/dftpy/properties/potential.py
 src/dftpy/td/__init__.py
 src/dftpy/td/casida.py
 src/dftpy/td/hamiltonian.py
 src/dftpy/td/interface.py
 src/dftpy/td/operator.py
```

