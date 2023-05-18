# Comparing `tmp/ape-foundry-0.6.7.tar.gz` & `tmp/ape-foundry-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-foundry-0.6.7.tar", last modified: Thu Apr 13 22:24:43 2023, max compression
+gzip compressed data, was "ape-foundry-0.6.8.tar", last modified: Thu May 18 18:15:26 2023, max compression
```

## Comparing `ape-foundry-0.6.7.tar` & `ape-foundry-0.6.8.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.675888 ape-foundry-0.6.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-13 22:24:43.675888 ape-foundry-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/ape_foundry/
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/ape_foundry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/ape_foundry/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/ape_foundry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27893 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/ape_foundry/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/ape_foundry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 22:24:43.000000 ape-foundry-0.6.7/ape_foundry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.667888 ape-foundry-0.6.7/ape_foundry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-13 22:24:43.000000 ape-foundry-0.6.7/ape_foundry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-04-13 22:24:43.000000 ape-foundry-0.6.7/ape_foundry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:24:43.000000 ape-foundry-0.6.7/ape_foundry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:24:43.000000 ape-foundry-0.6.7/ape_foundry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-13 22:24:43.000000 ape-foundry-0.6.7/ape_foundry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 22:24:43.000000 ape-foundry-0.6.7/ape_foundry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-13 22:24:43.675888 ape-foundry-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.667888 ape-foundry-0.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/tests/data/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/tests/data/contracts/ethereum/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.667888 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/
--rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/contract_a.json
--rw-r--r--   0 runner    (1001) docker     (123)    27536 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/contract_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/contract_c.json
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/has_error.json
--rw-r--r--   0 runner    (1001) docker     (123)    26899 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/reverts_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/solidity_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/token_a.json
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/token_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/local/vyper_contract.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.663888 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.675888 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
--rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
--rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
--rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
--rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
--rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.675888 ape-foundry-0.6.7/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/python/pytest_test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/python/pytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:43.675888 ape-foundry-0.6.7/tests/data/sources/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/sources/RevertsContractVy.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/sources/TokenA.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/data/sources/TokenB.vy
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/expected_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/test_fork_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/test_gas_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-13 22:23:49.000000 ape-foundry-0.6.7/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.413430 ape-foundry-0.6.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-18 18:15:26.413430 ape-foundry-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/ape_foundry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/ape_foundry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/ape_foundry/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/ape_foundry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30876 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/ape_foundry/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/ape_foundry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 18:15:26.000000 ape-foundry-0.6.8/ape_foundry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.405429 ape-foundry-0.6.8/ape_foundry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-18 18:15:26.000000 ape-foundry-0.6.8/ape_foundry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-05-18 18:15:26.000000 ape-foundry-0.6.8/ape_foundry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:15:26.000000 ape-foundry-0.6.8/ape_foundry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:15:26.000000 ape-foundry-0.6.8/ape_foundry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-18 18:15:26.000000 ape-foundry-0.6.8/ape_foundry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 18:15:26.000000 ape-foundry-0.6.8/ape_foundry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-18 18:15:26.413430 ape-foundry-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.405429 ape-foundry-0.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/tests/data/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/tests/data/contracts/ethereum/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.405429 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/
+-rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/contract_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27536 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/contract_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/contract_c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/has_error.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26899 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/reverts_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/solidity_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/token_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/token_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/local/vyper_contract.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.401430 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.409430 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.413430 ape-foundry-0.6.8/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/python/pytest_test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/python/pytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:26.413430 ape-foundry-0.6.8/tests/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/sources/RevertsContractVy.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/sources/TokenA.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/data/sources/TokenB.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/expected_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/test_fork_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/test_gas_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-18 18:14:28.000000 ape-foundry-0.6.8/tests/test_trace.py
```

### Comparing `ape-foundry-0.6.7/.github/ISSUE_TEMPLATE/bug.md` & `ape-foundry-0.6.8/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/.github/ISSUE_TEMPLATE/feature.md` & `ape-foundry-0.6.8/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/.github/ISSUE_TEMPLATE/work-item.md` & `ape-foundry-0.6.8/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/.github/release-drafter.yml` & `ape-foundry-0.6.8/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/.github/workflows/codeql.yml` & `ape-foundry-0.6.8/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/.github/workflows/commitlint.yaml` & `ape-foundry-0.6.8/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/.github/workflows/prtitle.yaml` & `ape-foundry-0.6.8/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/.github/workflows/publish.yaml` & `ape-foundry-0.6.8/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/.github/workflows/stale-prs.yml` & `ape-foundry-0.6.8/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/.github/workflows/test.yaml` & `ape-foundry-0.6.8/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/.gitignore` & `ape-foundry-0.6.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/.pre-commit-config.yaml` & `ape-foundry-0.6.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/CONTRIBUTING.md` & `ape-foundry-0.6.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/LICENSE` & `ape-foundry-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/PKG-INFO` & `ape-foundry-0.6.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: ape-foundry
-Version: 0.6.7
+Version: 0.6.8
 Summary: ape-foundry: Ape network provider for Foundry
 Home-page: https://github.com/ApeWorX/ape-foundry
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
         
-        Foundry network provider plugin for Ape. Foundry is a development framework written in Rust for Ethereum that includes a local network implementation.
+        Foundry network provider plugin for Ape.
+        Foundry is a development framework written in Rust for Ethereum that includes a local network implementation.
         
         ## Dependencies
         
         - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
         - Foundry. See Foundry's [Installation](https://github.com/foundry-rs/foundry#installation) documentation for steps.
         
         ## Installation
@@ -61,15 +62,16 @@
         foundry:
           request_timeout: 20  # Defaults to 30
           fork_request_timeout: 600  # Defaults to 300
         ```
         
         ## Mainnet Fork
         
-        The `ape-foundry` plugin also includes a mainnet fork provider. It requires using another provider that has access to mainnet.
+        The `ape-foundry` plugin also includes a mainnet fork provider.
+        It requires using another provider that has access to mainnet.
         
         Use it in most commands like this:
         
         ```bash
         ape console --network :mainnet-fork:foundry
         ```
         
@@ -80,36 +82,48 @@
           fork:
             ethereum:
               mainnet:
                 upstream_provider: alchemy
         
         ```
         
-        Otherwise, it defaults to the default mainnet provider plugin. You can also specify a `block_number` and `evm_version`.
+        Otherwise, it defaults to the default mainnet provider plugin.
+        You can also specify a `block_number` and `evm_version`.
         
         If the block number is specified, but no EVM version is specified, it is automatically set based on the block height for known networks.
         
         **NOTE**: Make sure you have the upstream provider plugin installed for ape.
         
         ```bash
         ape plugins install alchemy
         ```
         
+        ## Remote Anvil Node
+        
+        To connect to a remote anvil node, set up your config like this:
+        
+        ```yaml
+        foundry:
+          host: https://anvil.example.com
+        ```
+        
+        Now, instead of launching a local process, it will attempt to connect to the remote anvil node and use this plugin as the ape interface.
+        
 Keywords: ethereum
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
```

### Comparing `ape-foundry-0.6.7/README.md` & `ape-foundry-0.6.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Quick Start
 
-Foundry network provider plugin for Ape. Foundry is a development framework written in Rust for Ethereum that includes a local network implementation.
+Foundry network provider plugin for Ape.
+Foundry is a development framework written in Rust for Ethereum that includes a local network implementation.
 
 ## Dependencies
 
 - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
 - Foundry. See Foundry's [Installation](https://github.com/foundry-rs/foundry#installation) documentation for steps.
 
 ## Installation
@@ -53,15 +54,16 @@
 foundry:
   request_timeout: 20  # Defaults to 30
   fork_request_timeout: 600  # Defaults to 300
 ```
 
 ## Mainnet Fork
 
-The `ape-foundry` plugin also includes a mainnet fork provider. It requires using another provider that has access to mainnet.
+The `ape-foundry` plugin also includes a mainnet fork provider.
+It requires using another provider that has access to mainnet.
 
 Use it in most commands like this:
 
 ```bash
 ape console --network :mainnet-fork:foundry
 ```
 
@@ -72,16 +74,28 @@
   fork:
     ethereum:
       mainnet:
         upstream_provider: alchemy
 
 ```
 
-Otherwise, it defaults to the default mainnet provider plugin. You can also specify a `block_number` and `evm_version`.
+Otherwise, it defaults to the default mainnet provider plugin.
+You can also specify a `block_number` and `evm_version`.
 
 If the block number is specified, but no EVM version is specified, it is automatically set based on the block height for known networks.
 
 **NOTE**: Make sure you have the upstream provider plugin installed for ape.
 
 ```bash
 ape plugins install alchemy
 ```
+
+## Remote Anvil Node
+
+To connect to a remote anvil node, set up your config like this:
+
+```yaml
+foundry:
+  host: https://anvil.example.com
+```
+
+Now, instead of launching a local process, it will attempt to connect to the remote anvil node and use this plugin as the ape interface.
```

### Comparing `ape-foundry-0.6.7/ape_foundry/__init__.py` & `ape-foundry-0.6.8/ape_foundry/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/ape_foundry/constants.py` & `ape-foundry-0.6.8/ape_foundry/constants.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/ape_foundry/exceptions.py` & `ape-foundry-0.6.8/ape_foundry/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,12 +16,9 @@
 class FoundryNotInstalledError(FoundrySubprocessError):
     """
     Raised when Foundry is not installed.
     """
 
     def __init__(self):
         super().__init__(
-            "Missing local Foundry node client. "
-            "See ape-foundry README for install steps. "
-            "Note: global installation of Foundry will not work and "
-            "you must be in your project's directory."
+            "Missing local Foundry node client. See ape-foundry README for install steps."
         )
```

### Comparing `ape-foundry-0.6.7/ape_foundry/provider.py` & `ape-foundry-0.6.8/ape_foundry/provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,35 +17,36 @@
     UpstreamProvider,
     Web3Provider,
 )
 from ape.exceptions import (
     APINotImplementedError,
     ContractLogicError,
     OutOfGasError,
-    ProviderError,
     SubprocessError,
     VirtualMachineError,
 )
 from ape.logging import logger
 from ape.types import AddressType, BlockID, CallTreeNode, ContractCode, SnapshotID, TraceFrame
 from ape.utils import cached_property
 from ape_test import Config as TestConfig
 from eth_typing import HexStr
-from eth_utils import add_0x_prefix, is_0x_prefixed, is_hex, to_checksum_address, to_hex
+from eth_utils import add_0x_prefix, is_0x_prefixed, is_hex, to_hex
 from evm_trace import CallType, ParityTraceList
 from evm_trace import TraceFrame as EvmTraceFrame
 from evm_trace import get_calltree_from_geth_trace, get_calltree_from_parity_trace
 from hexbytes import HexBytes
 from web3 import HTTPProvider, Web3
+from web3.exceptions import ContractCustomError
 from web3.exceptions import ContractLogicError as Web3ContractLogicError
 from web3.exceptions import ExtraDataLengthError
 from web3.gas_strategies.rpc import rpc_gas_price_strategy
 from web3.middleware import geth_poa_middleware
 from web3.middleware.validation import MAX_EXTRADATA_LENGTH
 from web3.types import TxParams
+from yarl import URL
 
 from ape_foundry.constants import EVM_VERSION_BY_NETWORK
 
 from .exceptions import FoundryNotInstalledError, FoundryProviderError, FoundrySubprocessError
 
 EPHEMERAL_PORTS_START = 49152
 EPHEMERAL_PORTS_END = 60999
@@ -57,18 +58,29 @@
     upstream_provider: Optional[str] = None
     block_number: Optional[int] = None
     evm_version: Optional[str] = None
 
 
 class FoundryNetworkConfig(PluginConfig):
     port: Optional[Union[int, Literal["auto"]]] = DEFAULT_PORT
+    """Deprecated. Use ``host`` config."""
+
+    host: Optional[Union[str, Literal["auto"]]] = None
+    """The host address or ``"auto"`` to use localhost with a random port (with attempts)."""
+
+    manage_process: bool = True
+    """
+    If ``True`` and the host is local and Anvil is not running, will attempt to start.
+    Defaults to ``True``. If ``host`` is remote, will not be able to start.
+    """
 
     # Retry strategy configs, try increasing these if you're getting FoundrySubprocessError
     request_timeout: int = 30
     fork_request_timeout: int = 300
+    process_attempts: int = 0
 
     # For setting the values in --fork and --fork-block-number command arguments.
     # Used only in FoundryForkProvider.
     # Mapping of ecosystem_name => network_name => FoundryForkConfig
     fork: Dict[str, Dict[str, FoundryForkConfig]] = {}
 
     class Config:
@@ -76,18 +88,22 @@
 
 
 def _call(*args):
     return call([*args], stderr=PIPE, stdout=PIPE, stdin=PIPE)
 
 
 class FoundryProvider(SubprocessProvider, Web3Provider, TestProviderAPI):
-    port: Optional[int] = None
+    _host: Optional[str] = None
     attempted_ports: List[int] = []
-    unlocked_accounts: List[AddressType] = []
     cached_chain_id: Optional[int] = None
+    _did_warn_wrong_node = False
+
+    @property
+    def unlocked_accounts(self) -> List[AddressType]:
+        return list(self.account_manager.test_accounts._impersonated_accounts)
 
     @property
     def mnemonic(self) -> str:
         return self._test_config.mnemonic
 
     @property
     def number_of_accounts(self) -> int:
@@ -98,14 +114,22 @@
         return "anvil"
 
     @property
     def timeout(self) -> int:
         return self.config.request_timeout
 
     @property
+    def _clean_uri(self) -> str:
+        return str(URL(self.uri).with_user(None).with_password(None))
+
+    @property
+    def _port(self) -> Optional[int]:
+        return URL(self.uri).port
+
+    @property
     def chain_id(self) -> int:
         if self.cached_chain_id is not None:
             return self.cached_chain_id
 
         elif self.cached_chain_id is None and hasattr(self.web3, "eth"):
             self.cached_chain_id = self.web3.eth.chain_id
             return self.cached_chain_id
@@ -128,49 +152,78 @@
 
     @property
     def project_folder(self) -> Path:
         return self.config_manager.PROJECT_FOLDER
 
     @property
     def uri(self) -> str:
-        if not self.port:
-            raise FoundryProviderError("Can't build URI before `connect()` is called.")
+        if self._host is None:
+            self._host = self.config.host or f"http://127.0.0.1:{DEFAULT_PORT}"
 
-        return f"http://127.0.0.1:{self.port}"
+        return self._host
 
     @property
     def priority_fee(self) -> int:
         return self.conversion_manager.convert("2 gwei", int)
 
     @property
     def is_connected(self) -> bool:
+        if self._host in ("auto", None):
+            # Hasn't tried yet.
+            return False
+
         self._set_web3()
         return self._web3 is not None
 
     @cached_property
     def _test_config(self) -> TestConfig:
         return cast(TestConfig, self.config_manager.get_config("test"))
 
     def connect(self):
         """
         Start the foundry process and verify it's up and accepting connections.
         **NOTE**: Must set port before calling 'super().connect()'.
         """
 
-        if not self.port:
-            self.port = self.provider_settings.get("port", self.config.port)
+        warning = "`port` setting is deprecated. Please use `host` key that includes the port."
+        if "port" in self.provider_settings:
+            # TODO: Can remove after 0.7.
+            logger.warning(warning)
+            self._host = f"http://127.0.0.1:{self.provider_settings['port']}"
+
+        elif self.config.port != DEFAULT_PORT and self.config.host is not None:
+            raise FoundryProviderError(
+                "Cannot use deprecated `port` field with `host`. "
+                "Place `port` at end of `host` instead."
+            )
+
+        elif self.config.port != DEFAULT_PORT:
+            # We only get here if the user configured a port without a host,
+            # the old way of doing it. TODO: Can remove after 0.7.
+            logger.warning(warning)
+            if self.config.port not in (None, "auto"):
+                self._host = f"http://127.0.0.1:{self.config.port}"
+            else:
+                # This will trigger selecting a random port on localhost and trying.
+                self._host = "auto"
+
+        elif "host" in self.provider_settings:
+            self._host = self.provider_settings["host"]
+
+        elif self._host is None:
+            self._host = self.config.host or f"http://127.0.0.1:{DEFAULT_PORT}"
 
         if self.is_connected:
             # Connects to already running process
             self._start()
-        else:
+
+        elif self.config.manage_process:
             # Only do base-process setup if not connecting to already-running process
             super().connect()
-
-            if self.port:
+            if self._host:
                 self._set_web3()
                 if not self._web3:
                     # Process attempts to get started at this point.
                     self._start()
                     if not self.stdout_logs_path.is_file():
                         # Process output not being captured
                         return
@@ -182,52 +235,62 @@
                         logged_lines = [x for x in self.stdout_logs_path.read_text().split("\n")]
                         for line in logged_lines:
                             if line.startswith(wait_for_key):
                                 return
 
                         iterations += 1
                         if iterations == timeout:
-                            raise ProviderError("Timed-out waiting for process to begin listening.")
+                            raise FoundryProviderError(
+                                "Timed-out waiting for process to begin listening."
+                            )
 
                 else:
-                    # The user configured a port and the anvil process was already running.
+                    # The user configured a host and the anvil process was already running.
                     logger.info(
-                        f"Connecting to existing '{self.process_name}' at port '{self.port}'."
+                        f"Connecting to existing '{self.process_name}' "
+                        f"at host '{self._clean_uri}'."
                     )
             else:
                 for _ in range(self.config.process_attempts):
                     try:
                         self._start()
                         break
                     except FoundryNotInstalledError:
                         # Is a sub-class of `FoundrySubprocessError` but we to still raise
                         # so we don't keep retrying.
                         raise
                     except SubprocessError as exc:
                         logger.info("Retrying anvil subprocess startup: %r", exc)
-                        self.port = None
+                        self._host = None
+        else:
+            raise FoundryProviderError(
+                f"Failed to connect to remote Anvil node at '{self._clean_uri}'."
+            )
 
     def _set_web3(self):
-        if not self.port:
+        if not self._host:
             return
 
         self._web3 = Web3(HTTPProvider(self.uri, request_kwargs={"timeout": self.timeout}))
         if not self._web3.is_connected():
             self._web3 = None
             return
 
         # Verify is actually a Foundry provider,
         # or else skip it to possibly try another port.
         client_version = self._web3.client_version.lower()
         if "anvil" in client_version:
             self._web3.eth.set_gas_price_strategy(rpc_gas_price_strategy)
-        else:
-            raise ProviderError(
-                f"Port '{self.port}' already in use by another process that isn't an Anvil node."
+        elif self._port is not None:
+            raise FoundryProviderError(
+                f"Port '{self._port}' already in use by another process that isn't an Anvil node."
             )
+        else:
+            # Not sure if possible to get here.
+            raise FoundryProviderError("Failed to start Anvil process.")
 
         def check_poa(block_id) -> bool:
             try:
                 block = self.web3.eth.get_block(block_id)
             except ExtraDataLengthError:
                 return True
             else:
@@ -237,68 +300,67 @@
                 )
 
         # Handle if using PoA
         if any(map(check_poa, (0, "latest"))):
             self._web3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
     def _start(self):
-        use_random_port = self.port == "auto"
+        use_random_port = self.uri == "auto"
         if use_random_port:
-            self.port = None
+            self._host = None
 
             if DEFAULT_PORT not in self.attempted_ports and not use_random_port:
-                self.port = DEFAULT_PORT
+                # First, attempt the default port before anything else.
+                self._host = f"127.0.0.1:{DEFAULT_PORT}"
+
             else:
+                # Pick a random port
                 port = random.randint(EPHEMERAL_PORTS_START, EPHEMERAL_PORTS_END)
                 max_attempts = 25
                 attempts = 0
                 while port in self.attempted_ports:
                     port = random.randint(EPHEMERAL_PORTS_START, EPHEMERAL_PORTS_END)
                     attempts += 1
                     if attempts == max_attempts:
                         ports_str = ", ".join([str(p) for p in self.attempted_ports])
                         raise FoundryProviderError(
                             f"Unable to find an available port. Ports tried: {ports_str}"
                         )
 
-                self.port = port
+                self.attempted_ports.append(port)
+                self._host = f"http://127.0.0.1:{port}"
+
+        elif ":" in self._host and self._port is not None:
+            # Append the one and only port to the attempted ports list, for honest keeping.
+            self.attempted_ports.append(self._port)
+
+        else:
+            self._host = f"http://127.0.0.1:{DEFAULT_PORT}"
 
-        self.attempted_ports.append(self.port)
         self.start()
 
     def disconnect(self):
         self._web3 = None
-        self.port = None
+        self._host = None
         super().disconnect()
 
     def build_command(self) -> List[str]:
         return [
             self.anvil_bin,
             "--port",
-            f"{self.port}",
+            f"{self._port or DEFAULT_PORT}",
             "--mnemonic",
             self.mnemonic,
             "--accounts",
             f"{self.number_of_accounts}",
             "--derivation-path",
             "m/44'/60'/0'",
             "--steps-tracing",
         ]
 
-    def estimate_gas_cost(self, txn: TransactionAPI, **kwargs) -> int:
-        txn_dict = txn.dict()
-
-        # Anvil is unable to handle integer-based type.
-        # https://github.com/foundry-rs/foundry/issues/4240
-        if isinstance(txn_dict.get("type"), int):
-            txn_dict["type"] = HexBytes(txn_dict["type"]).hex()
-
-        modified_txn = txn.__class__.construct(**txn_dict)
-        return super().estimate_gas_cost(modified_txn)
-
     def set_balance(self, account: AddressType, amount: Union[int, float, str, bytes]):
         is_str = isinstance(amount, str)
         _is_hex = False if not is_str else is_0x_prefixed(str(amount))
         is_key_word = is_str and len(str(amount).split(" ")) > 1
         if is_key_word:
             # This allows values such as "1000 ETH".
             amount = self.conversion_manager.convert(amount, int)
@@ -316,44 +378,42 @@
 
     def set_timestamp(self, new_timestamp: int):
         self._make_request("evm_setNextBlockTimestamp", [new_timestamp])
 
     def mine(self, num_blocks: int = 1):
         result = self._make_request("evm_mine", [{"blocks": num_blocks, "timestamp": None}])
         if result != "0x0":
-            raise ProviderError(f"Failed to mine.\n{result}")
+            raise FoundryProviderError(f"Failed to mine.\n{result}")
 
     def snapshot(self) -> str:
         return self._make_request("evm_snapshot", [])
 
     def revert(self, snapshot_id: SnapshotID) -> bool:
         if isinstance(snapshot_id, int):
             snapshot_id = HexBytes(snapshot_id).hex()
 
         result = self._make_request("evm_revert", [snapshot_id])
         return result is True
 
     def unlock_account(self, address: AddressType) -> bool:
         self._make_request("anvil_impersonateAccount", [address])
-        self.unlocked_accounts.append(address)
         return True
 
     def send_transaction(self, txn: TransactionAPI) -> ReceiptAPI:
         """
         Creates a new message call transaction or a contract creation
         for signed transactions.
         """
         sender = txn.sender
         if sender:
             sender = self.conversion_manager.convert(txn.sender, AddressType)
 
         if sender and sender in self.unlocked_accounts:
             # Allow for an unsigned transaction
-
-            sender = to_checksum_address(sender)  # For mypy
+            sender = cast(AddressType, sender)  # We know it's checksummed at this point.
             txn = self.prepare_transaction(txn)
             original_code = HexBytes(self.get_code(sender))
             if original_code:
                 self.set_code(sender, "")
 
             try:
                 txn_dict = txn.dict()
@@ -397,14 +457,18 @@
             txn_dict = receipt.transaction.dict()
             if isinstance(txn_dict.get("type"), int):
                 txn_dict["type"] = HexBytes(txn_dict["type"]).hex()
 
             txn_params = cast(TxParams, txn_dict)
 
             # Replay txn to get revert reason
+            # NOTE: For some reason, `nonce` can't be in the txn params or else it fails.
+            if "nonce" in txn_params:
+                del txn_params["nonce"]
+
             try:
                 self.web3.eth.call(txn_params)
             except Exception as err:
                 vm_err = self.get_virtual_machine_error(err, txn=txn)
                 vm_err.txn = txn
                 raise vm_err from err
 
@@ -417,15 +481,15 @@
         arguments = self._prepare_call(txn, **kwargs)
 
         if skip_trace:
             return self._eth_call(arguments)
 
         show_gas = kwargs.pop("show_gas_report", False)
         show_trace = kwargs.pop("show_trace", False)
-        track_gas = self.chain_manager._reports.track_gas
+        track_gas = self._test_runner is not None and self._test_runner.gas_tracker.enabled
         needs_trace = show_gas or show_trace or track_gas
         if not needs_trace:
             return self._eth_call(arguments)
 
         # The user is requesting information related to a call's trace,
         # such as gas usage data.
 
@@ -455,15 +519,16 @@
             call_tree.enrich()
 
         if track_gas and call_tree and receiver is not None:
             # Gas report being collected, likely for showing a report
             # at the end of a test run.
             # Use `in_place=False` in case also `show_trace=True`
             enriched_call_tree = call_tree.enrich(in_place=False)
-            self.chain_manager._reports.append_gas(enriched_call_tree, receiver)
+            if self._test_runner:
+                self._test_runner.gas_tracker.append_gas(enriched_call_tree, receiver)
 
         if show_gas:
             enriched_call_tree = call_tree.enrich(in_place=False)
             self.chain_manager._reports.show_gas(enriched_call_tree)
 
         if show_trace:
             call_tree = call_tree.enrich(use_symbol_for_tokens=True)
@@ -478,15 +543,15 @@
 
     def get_balance(self, address: str) -> int:
         if hasattr(address, "address"):
             address = address.address
 
         result = self._make_request("eth_getBalance", [address, "latest"])
         if not result:
-            raise ProviderError(f"Failed to get balance for account '{address}'.")
+            raise FoundryProviderError(f"Failed to get balance for account '{address}'.")
 
         return int(result, 16) if isinstance(result, str) else result
 
     def get_transaction_trace(self, txn_hash: str) -> Iterator[TraceFrame]:
         for trace in self._get_transaction_trace(txn_hash):
             yield self._create_trace_frame(trace)
 
@@ -499,15 +564,15 @@
             yield EvmTraceFrame(**frame)
 
     def get_call_tree(self, txn_hash: str) -> CallTreeNode:
         raw_trace_list = self._make_request("trace_transaction", [txn_hash])
         trace_list = ParityTraceList.parse_obj(raw_trace_list)
 
         if not trace_list:
-            raise ProviderError(f"No trace found for transaction '{txn_hash}'")
+            raise FoundryProviderError(f"No trace found for transaction '{txn_hash}'")
 
         evm_call = get_calltree_from_parity_trace(trace_list)
         return self._create_call_tree_node(evm_call, txn_hash=txn_hash)
 
     def get_virtual_machine_error(self, exception: Exception, **kwargs) -> VirtualMachineError:
         if not len(exception.args):
             return VirtualMachineError(base_err=exception, **kwargs)
@@ -559,14 +624,19 @@
         elif message == "Transaction ran out of gas":
             return OutOfGasError(**kwargs)
 
         elif message.startswith("execution reverted: "):
             err = ContractLogicError(message.replace("execution reverted: ", "").strip(), **kwargs)
             return self.compiler_manager.enrich_error(err)
 
+        elif isinstance(exception, ContractCustomError):
+            # Is raw hex (custom exception)
+            err = ContractLogicError(message, **kwargs)
+            return self.compiler_manager.enrich_error(err)
+
         return VirtualMachineError(message, **kwargs)
 
     def set_block_gas_limit(self, gas_limit: int) -> bool:
         return self._make_request("evm_setBlockGasLimit", [hex(gas_limit)]) is True
 
     def set_code(self, address: AddressType, code: ContractCode) -> bool:
         if isinstance(code, bytes):
@@ -688,15 +758,15 @@
             if isinstance(upstream_provider, Web3Provider):
                 logger.error(
                     f"Upstream provider '{upstream_provider.name}' missing Geth PoA middleware."
                 )
                 upstream_provider.web3.middleware_onion.inject(geth_poa_middleware, layer=0)
                 upstream_genesis_block_hash = upstream_provider.get_block(0).hash
             else:
-                raise ProviderError(f"Unable to get genesis block: {err}.") from err
+                raise FoundryProviderError(f"Unable to get genesis block: {err}.") from err
 
         upstream_provider.disconnect()
         if self.get_block(0).hash != upstream_genesis_block_hash:
             logger.warning(
                 "Upstream network has mismatching genesis block. "
                 "This could be an issue with foundry."
             )
@@ -706,15 +776,15 @@
             raise FoundryProviderError(
                 f"Provider '{self._upstream_provider.name}' is not an upstream provider."
             )
 
         if not self.fork_url:
             raise FoundryProviderError("Upstream provider does not have a ``connection_str``.")
 
-        if self.fork_url.replace("localhost", "127.0.0.1") == self.uri:
+        if self.fork_url.replace("localhost", "127.0.0.1").replace("http://", "") == self.uri:
             raise FoundryProviderError(
                 "Invalid upstream-fork URL. Can't be same as local anvil node."
             )
 
         cmd = super().build_command()
         cmd.extend(("--fork-url", self.fork_url))
         if self.fork_block_number is not None:
```

### Comparing `ape-foundry-0.6.7/ape_foundry.egg-info/PKG-INFO` & `ape-foundry-0.6.8/ape_foundry.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: ape-foundry
-Version: 0.6.7
+Version: 0.6.8
 Summary: ape-foundry: Ape network provider for Foundry
 Home-page: https://github.com/ApeWorX/ape-foundry
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
         
-        Foundry network provider plugin for Ape. Foundry is a development framework written in Rust for Ethereum that includes a local network implementation.
+        Foundry network provider plugin for Ape.
+        Foundry is a development framework written in Rust for Ethereum that includes a local network implementation.
         
         ## Dependencies
         
         - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
         - Foundry. See Foundry's [Installation](https://github.com/foundry-rs/foundry#installation) documentation for steps.
         
         ## Installation
@@ -61,15 +62,16 @@
         foundry:
           request_timeout: 20  # Defaults to 30
           fork_request_timeout: 600  # Defaults to 300
         ```
         
         ## Mainnet Fork
         
-        The `ape-foundry` plugin also includes a mainnet fork provider. It requires using another provider that has access to mainnet.
+        The `ape-foundry` plugin also includes a mainnet fork provider.
+        It requires using another provider that has access to mainnet.
         
         Use it in most commands like this:
         
         ```bash
         ape console --network :mainnet-fork:foundry
         ```
         
@@ -80,36 +82,48 @@
           fork:
             ethereum:
               mainnet:
                 upstream_provider: alchemy
         
         ```
         
-        Otherwise, it defaults to the default mainnet provider plugin. You can also specify a `block_number` and `evm_version`.
+        Otherwise, it defaults to the default mainnet provider plugin.
+        You can also specify a `block_number` and `evm_version`.
         
         If the block number is specified, but no EVM version is specified, it is automatically set based on the block height for known networks.
         
         **NOTE**: Make sure you have the upstream provider plugin installed for ape.
         
         ```bash
         ape plugins install alchemy
         ```
         
+        ## Remote Anvil Node
+        
+        To connect to a remote anvil node, set up your config like this:
+        
+        ```yaml
+        foundry:
+          host: https://anvil.example.com
+        ```
+        
+        Now, instead of launching a local process, it will attempt to connect to the remote anvil node and use this plugin as the ape interface.
+        
 Keywords: ethereum
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
```

### Comparing `ape-foundry-0.6.7/ape_foundry.egg-info/SOURCES.txt` & `ape-foundry-0.6.8/ape_foundry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/ape_foundry.egg-info/requires.txt` & `ape-foundry-0.6.8/ape_foundry.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-eth-ape<0.7,>=0.6.8
+eth-ape<0.7,>=0.6.9
 evm-trace
 hexbytes
 web3
+yarl
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
 ape-alchemy
```

### Comparing `ape-foundry-0.6.7/pyproject.toml` & `ape-foundry-0.6.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/setup.py` & `ape-foundry-0.6.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,20 +65,21 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-foundry",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.6.8,<0.7",
-        "evm-trace",  # Use same version as eth-ape
-        "hexbytes",  # Use same version as eth-ape
-        "web3",  # Use same version as eth-ape
+        "eth-ape>=0.6.9,<0.7",
+        "evm-trace",  # Use same version as ape
+        "hexbytes",  # Use same version as ape
+        "web3",  # Use same version as ape
+        "yarl",  # Use same version as ape
     ],
-    python_requires=">=3.8,<3.11",
+    python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_foundry"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_foundry": ["py.typed"]},
```

### Comparing `ape-foundry-0.6.7/tests/ape-config.yaml` & `ape-foundry-0.6.8/tests/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/conftest.py` & `ape-foundry-0.6.8/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,28 +199,28 @@
 def mainnet_fork_port():
     return MAINNET_FORK_PORT
 
 
 @pytest.fixture
 def mainnet_fork_provider(name, networks, mainnet_fork_port):
     with networks.ethereum.mainnet_fork.use_provider(
-        name, provider_settings={"port": mainnet_fork_port}
+        name, provider_settings={"host": f"http://127.0.0.1:{mainnet_fork_port}"}
     ) as provider:
         yield provider
 
 
 @pytest.fixture
 def goerli_fork_port():
     return GOERLI_FORK_PORT
 
 
 @pytest.fixture
 def goerli_fork_provider(name, networks, goerli_fork_port):
     with networks.ethereum.goerli_fork.use_provider(
-        name, provider_settings={"port": goerli_fork_port}
+        name, provider_settings={"host": f"http://127.0.0.1:{goerli_fork_port}"}
     ) as provider:
         yield provider
 
 
 @pytest.fixture(scope="session")
 def temp_config(config):
     @contextmanager
```

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/contract_a.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/contract_a.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/contract_b.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/contract_b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/contract_c.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/contract_c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/has_error.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/has_error.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/reverts_contract.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/reverts_contract.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/solidity_contract.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/solidity_contract.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/token_a.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/token_a.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/token_b.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/token_b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/local/vyper_contract.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/local/vyper_contract.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json` & `ape-foundry-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/python/pytest_tests.py` & `ape-foundry-0.6.8/tests/data/python/pytest_tests.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/sources/RevertsContractVy.vy` & `ape-foundry-0.6.8/tests/data/sources/RevertsContractVy.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/sources/TokenA.vy` & `ape-foundry-0.6.8/tests/data/sources/TokenA.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/data/sources/TokenB.vy` & `ape-foundry-0.6.8/tests/data/sources/TokenB.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/expected_traces.py` & `ape-foundry-0.6.8/tests/expected_traces.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/test_fork_provider.py` & `ape-foundry-0.6.8/tests/test_fork_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,39 +16,42 @@
     return owner.deploy(contract_container)
 
 
 @pytest.mark.fork
 def test_multiple_providers(
     name, networks, connected_provider, mainnet_fork_port, goerli_fork_port
 ):
+    default_host = "http://127.0.0.1:8545"
     assert networks.active_provider.name == name
     assert networks.active_provider.network.name == LOCAL_NETWORK_NAME
-    assert networks.active_provider.port == 8545
+    assert networks.active_provider.uri == default_host
+    mainnet_fork_host = f"http://127.0.0.1:{mainnet_fork_port}"
 
     with networks.ethereum.mainnet_fork.use_provider(
-        name, provider_settings={"port": mainnet_fork_port}
+        name, provider_settings={"host": mainnet_fork_host}
     ):
         assert networks.active_provider.name == name
         assert networks.active_provider.network.name == "mainnet-fork"
-        assert networks.active_provider.port == mainnet_fork_port
+        assert networks.active_provider.uri == mainnet_fork_host
+        goerli_fork_host = f"http://127.0.0.1:{goerli_fork_port}"
 
         with networks.ethereum.goerli_fork.use_provider(
-            name, provider_settings={"port": goerli_fork_port}
+            name, provider_settings={"host": goerli_fork_host}
         ):
             assert networks.active_provider.name == name
             assert networks.active_provider.network.name == "goerli-fork"
-            assert networks.active_provider.port == goerli_fork_port
+            assert networks.active_provider.uri == goerli_fork_host
 
         assert networks.active_provider.name == name
         assert networks.active_provider.network.name == "mainnet-fork"
-        assert networks.active_provider.port == mainnet_fork_port
+        assert networks.active_provider.uri == mainnet_fork_host
 
     assert networks.active_provider.name == name
     assert networks.active_provider.network.name == LOCAL_NETWORK_NAME
-    assert networks.active_provider.port == 8545
+    assert networks.active_provider.uri == default_host
 
 
 @pytest.mark.parametrize("network", [k for k in NETWORKS.keys()])
 def test_fork_config(name, config, network):
     plugin_config = config.get_config(name)
     network_config = plugin_config["fork"].get("ethereum", {}).get(network, {})
     message = f"Config not registered for network '{network}'."
@@ -141,21 +144,28 @@
 @pytest.mark.fork
 def test_transaction_contract_as_sender(
     mainnet_fork_contract_instance, mainnet_fork_provider, convert
 ):
     # Set balance so test wouldn't normally fail from lack of funds
     mainnet_fork_provider.set_balance(mainnet_fork_contract_instance.address, "1000 ETH")
     with pytest.raises(ContractLogicError, match="!authorized"):
-        mainnet_fork_contract_instance.setNumber(10, sender=mainnet_fork_contract_instance)
+        # NOTE: For some reason, this only fails when for estimate gas. Otherwise, the status
+        # is non-failing. This wasn't happened prior to Ape 0.6.9 because a bugfix revealed
+        # that the test config was never getting applied and thus we never hit this problem
+        # because it was estimating gas before (even tho should have been using max).
+        mainnet_fork_contract_instance.setNumber(
+            10, sender=mainnet_fork_contract_instance, gas="auto"
+        )
 
 
 @pytest.mark.fork
 def test_transaction_unknown_contract_as_sender(accounts, mainnet_fork_provider):
     account = "0xFEB4acf3df3cDEA7399794D0869ef76A6EfAff52"
     multi_sig = accounts[account]
+    multi_sig.balance += accounts.conversion_manager.convert("1000 ETH", int)
     receipt = multi_sig.transfer(accounts[0], "100 gwei")
     assert not receipt.failed
 
 
 @pytest.mark.fork
 def test_get_receipt(mainnet_fork_provider, mainnet_fork_contract_instance, owner):
     receipt = mainnet_fork_contract_instance.setAddress(owner.address, sender=owner)
```

### Comparing `ape-foundry-0.6.7/tests/test_gas_report.py` & `ape-foundry-0.6.8/tests/test_gas_report.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.7/tests/test_provider.py` & `ape-foundry-0.6.8/tests/test_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 import pytest
 from ape.exceptions import ContractLogicError
 from ape.pytest.contextmanagers import RevertsContextManager as reverts
 from ape.types import CallTreeNode, TraceFrame
 from evm_trace import CallType
 from hexbytes import HexBytes
 
-from ape_foundry.exceptions import FoundryProviderError
 from ape_foundry.provider import FOUNDRY_CHAIN_ID
 
 TEST_WALLET_ADDRESS = "0xD9b7fdb3FC0A0Aa3A507dCf0976bc23D49a9C7A3"
 
 
 def test_instantiation(disconnected_provider, name):
     assert disconnected_provider.name == name
 
 
 def test_connect_and_disconnect(disconnected_provider):
     # Use custom port to prevent connecting to a port used in another test.
 
-    disconnected_provider.port = 8555
+    disconnected_provider._host = "http://127.0.0.1:8555"
     disconnected_provider.connect()
 
     try:
         assert disconnected_provider.is_connected
         assert disconnected_provider.chain_id == FOUNDRY_CHAIN_ID
     finally:
         disconnected_provider.disconnect()
@@ -36,23 +35,19 @@
 
 def test_gas_price(connected_provider):
     gas_price = connected_provider.gas_price
     assert gas_price > 1
 
 
 def test_uri_disconnected(disconnected_provider):
-    with pytest.raises(
-        FoundryProviderError, match=r"Can't build URI before `connect\(\)` is called\."
-    ):
-        _ = disconnected_provider.uri
+    assert disconnected_provider.uri == "http://127.0.0.1:8545"
 
 
 def test_uri(connected_provider):
-    expected_uri = f"http://127.0.0.1:{connected_provider.port}"
-    assert expected_uri in connected_provider.uri
+    assert connected_provider.uri in connected_provider.uri
 
 
 def test_set_block_gas_limit(connected_provider):
     gas_limit = connected_provider.get_block("latest").gas_limit
     assert connected_provider.set_block_gas_limit(gas_limit) is True
 
 
@@ -91,18 +86,17 @@
 
     connected_provider.revert(snap)
     block_3 = connected_provider.get_block("latest")
     assert block_1.number == block_3.number
     assert block_1.hash == block_3.hash
 
 
-def test_unlock_account(connected_provider):
+def test_unlock_account(connected_provider, accounts):
     actual = connected_provider.unlock_account(TEST_WALLET_ADDRESS)
     assert actual is True
-    assert TEST_WALLET_ADDRESS in connected_provider.unlocked_accounts
 
 
 def test_get_transaction_trace(connected_provider, contract_instance, owner):
     receipt = contract_instance.setNumber(10, sender=owner)
 
     # Indirectly calls `connected_provider.get_transaction_trace()`
     frame_data = list(receipt.trace)
@@ -208,7 +202,14 @@
 
 def test_revert_error(error_contract, not_owner):
     """
     Test matching a revert custom Solidity error.
     """
     with pytest.raises(error_contract.Unauthorized):
         error_contract.withdraw(sender=not_owner)
+
+
+def test_host(temp_config, networks):
+    data = {"foundry": {"host": "https://example.com"}}
+    with temp_config(data):
+        provider = networks.ethereum.local.get_provider("foundry")
+        assert provider.uri == "https://example.com"
```

### Comparing `ape-foundry-0.6.7/tests/test_trace.py` & `ape-foundry-0.6.8/tests/test_trace.py`

 * *Files identical despite different names*

