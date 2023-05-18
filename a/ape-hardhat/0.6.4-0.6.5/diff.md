# Comparing `tmp/ape-hardhat-0.6.4.tar.gz` & `tmp/ape-hardhat-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-hardhat-0.6.4.tar", last modified: Thu Apr 13 22:08:51 2023, max compression
+gzip compressed data, was "ape-hardhat-0.6.5.tar", last modified: Thu May 18 18:15:47 2023, max compression
```

## Comparing `ape-hardhat-0.6.4.tar` & `ape-hardhat-0.6.5.tar`

### file list

```diff
@@ -1,131 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.781949 ape-hardhat-0.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.773949 ape-hardhat-0.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.773949 ape-hardhat-0.6.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.773949 ape-hardhat-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-13 22:08:51.781949 ape-hardhat-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.773949 ape-hardhat-0.6.4/ape_hardhat/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/ape_hardhat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/ape_hardhat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/ape_hardhat/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/ape_hardhat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 22:08:51.000000 ape-hardhat-0.6.4/ape_hardhat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.773949 ape-hardhat-0.6.4/ape_hardhat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-13 22:08:51.000000 ape-hardhat-0.6.4/ape_hardhat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-04-13 22:08:51.000000 ape-hardhat-0.6.4/ape_hardhat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:08:51.000000 ape-hardhat-0.6.4/ape_hardhat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:08:51.000000 ape-hardhat-0.6.4/ape_hardhat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-13 22:08:51.000000 ape-hardhat-0.6.4/ape_hardhat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 22:08:51.000000 ape-hardhat-0.6.4/ape_hardhat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/hardhat.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-13 22:08:51.781949 ape-hardhat-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.773949 ape-hardhat-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.769949 ape-hardhat-0.6.4/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.769949 ape-hardhat-0.6.4/tests/data/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.769949 ape-hardhat-0.6.4/tests/data/contracts/ethereum/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.777949 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/
--rw-r--r--   0 runner    (1001) docker     (123)    28685 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/contract_a.json
--rw-r--r--   0 runner    (1001) docker     (123)    27534 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/contract_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/contract_c.json
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/has_error.json
--rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/solidity_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/token_a.json
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/token_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/vyper_contract.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.769949 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.781949 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
--rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
--rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
--rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
--rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
--rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.781949 ape-hardhat-0.6.4/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/python/pytest_test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/python/pytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:08:51.781949 ape-hardhat-0.6.4/tests/data/sources/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/sources/TokenA.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/data/sources/TokenB.vy
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/expected_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/test_fork_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/test_gas_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-13 22:08:01.000000 ape-hardhat-0.6.4/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.733898 ape-hardhat-0.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.721898 ape-hardhat-0.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.721898 ape-hardhat-0.6.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.721898 ape-hardhat-0.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-18 18:15:47.733898 ape-hardhat-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.725898 ape-hardhat-0.6.5/ape_hardhat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/ape_hardhat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/ape_hardhat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25949 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/ape_hardhat/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/ape_hardhat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 18:15:47.000000 ape-hardhat-0.6.5/ape_hardhat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.725898 ape-hardhat-0.6.5/ape_hardhat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-18 18:15:47.000000 ape-hardhat-0.6.5/ape_hardhat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-05-18 18:15:47.000000 ape-hardhat-0.6.5/ape_hardhat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:15:47.000000 ape-hardhat-0.6.5/ape_hardhat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:15:47.000000 ape-hardhat-0.6.5/ape_hardhat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-18 18:15:47.000000 ape-hardhat-0.6.5/ape_hardhat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 18:15:47.000000 ape-hardhat-0.6.5/ape_hardhat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/hardhat.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-18 18:15:47.733898 ape-hardhat-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.725898 ape-hardhat-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.721898 ape-hardhat-0.6.5/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.721898 ape-hardhat-0.6.5/tests/data/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.721898 ape-hardhat-0.6.5/tests/data/contracts/ethereum/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.725898 ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/
+-rw-r--r--   0 runner    (1001) docker     (123)    28685 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/contract_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27534 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/contract_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/contract_c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/has_error.json
+-rw-r--r--   0 runner    (1001) docker     (123)    45606 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/reverts_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/solidity_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/sub_reverts_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/token_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/token_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/vyper_contract.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.721898 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.733898 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.733898 ape-hardhat-0.6.5/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/python/pytest_test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/python/pytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.733898 ape-hardhat-0.6.5/tests/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/sources/RevertsContractVy.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/sources/SubRevertsVy.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/sources/TokenA.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/sources/TokenB.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:15:47.733898 ape-hardhat-0.6.5/tests/data/sources/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/data/sources/interfaces/ISubRevertsVy.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/expected_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/test_fork_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/test_gas_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-18 18:14:44.000000 ape-hardhat-0.6.5/tests/test_trace.py
```

### Comparing `ape-hardhat-0.6.4/.github/ISSUE_TEMPLATE/bug.md` & `ape-hardhat-0.6.5/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/.github/ISSUE_TEMPLATE/feature.md` & `ape-hardhat-0.6.5/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/.github/ISSUE_TEMPLATE/work-item.md` & `ape-hardhat-0.6.5/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/.github/release-drafter.yml` & `ape-hardhat-0.6.5/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/.github/workflows/codeql.yml` & `ape-hardhat-0.6.5/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/.github/workflows/commit.yaml` & `ape-hardhat-0.6.5/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/.github/workflows/prtitle.yaml` & `ape-hardhat-0.6.5/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/.github/workflows/publish.yaml` & `ape-hardhat-0.6.5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/.github/workflows/stale-prs.yml` & `ape-hardhat-0.6.5/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/.github/workflows/test.yaml` & `ape-hardhat-0.6.5/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/.gitignore` & `ape-hardhat-0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/.pre-commit-config.yaml` & `ape-hardhat-0.6.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/CONTRIBUTING.md` & `ape-hardhat-0.6.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/LICENSE` & `ape-hardhat-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/PKG-INFO` & `ape-hardhat-0.6.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-hardhat
-Version: 0.6.4
+Version: 0.6.5
 Summary: ape-hardhat: Ape network provider for Hardhat
 Home-page: https://github.com/ApeWorX/ape-hardhat
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
         
@@ -105,14 +105,27 @@
                 enable_hardhat_deployments: true
         ```
         
         ```bash
         ape plugins install alchemy
         ```
         
+        ## Custom Hardhat Config File
+        
+        By default, Ape generates and uses a basic config file for starting up a Hardhat node and having the same test accounts that Ape expects.
+        To avoid conflict with other pre-existing Hardhat config files, Ape generates one in `$HOME/.ape/hardhat` and always refers to that one.
+        To use a different one, such as the one in your local project instead, add the following to your `ape-config.yaml`:
+        
+        ```yaml
+        hardhat:
+          hardhat_config_file: ./hardhat.config.ts
+        ```
+        
+        **NOTE**: You can refer to either a Hardhat JS file or a Hardhat TS file.
+        
         ## Development
         
         Please see the [contributing guide](CONTRIBUTING.md) to learn more how to contribute to this project.
         Comments, questions, criticisms and pull requests are welcomed.
         
 Keywords: ethereum
 Platform: UNKNOWN
```

### Comparing `ape-hardhat-0.6.4/README.md` & `ape-hardhat-0.6.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -97,11 +97,24 @@
         enable_hardhat_deployments: true
 ```
 
 ```bash
 ape plugins install alchemy
 ```
 
+## Custom Hardhat Config File
+
+By default, Ape generates and uses a basic config file for starting up a Hardhat node and having the same test accounts that Ape expects.
+To avoid conflict with other pre-existing Hardhat config files, Ape generates one in `$HOME/.ape/hardhat` and always refers to that one.
+To use a different one, such as the one in your local project instead, add the following to your `ape-config.yaml`:
+
+```yaml
+hardhat:
+  hardhat_config_file: ./hardhat.config.ts
+```
+
+**NOTE**: You can refer to either a Hardhat JS file or a Hardhat TS file.
+
 ## Development
 
 Please see the [contributing guide](CONTRIBUTING.md) to learn more how to contribute to this project.
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-hardhat-0.6.4/ape_hardhat/__init__.py` & `ape-hardhat-0.6.5/ape_hardhat/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/ape_hardhat/exceptions.py` & `ape-hardhat-0.6.5/ape_hardhat/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/ape_hardhat/provider.py` & `ape-hardhat-0.6.5/ape_hardhat/provider.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import json
 import random
 import re
 import shutil
 from pathlib import Path
-from subprocess import PIPE, call
+from subprocess import PIPE, CalledProcessError, call, check_output
 from typing import Dict, Iterator, List, Literal, Optional, Union, cast
 
 from ape.api import (
     PluginConfig,
     ProviderAPI,
     ReceiptAPI,
     SubprocessProvider,
@@ -15,22 +16,24 @@
     UpstreamProvider,
     Web3Provider,
 )
 from ape.exceptions import (
     ContractLogicError,
     OutOfGasError,
     ProviderError,
+    RPCTimeoutError,
     SubprocessError,
     TransactionError,
     VirtualMachineError,
 )
 from ape.logging import logger
 from ape.types import AddressType, CallTreeNode, ContractCode, SnapshotID, TraceFrame
 from ape.utils import cached_property
 from ape_test import Config as TestConfig
+from chompjs import parse_js_object  # type: ignore
 from eth_utils import is_0x_prefixed, is_hex, to_hex
 from evm_trace import CallType
 from evm_trace import TraceFrame as EvmTraceFrame
 from evm_trace import get_calltree_from_geth_trace
 from hexbytes import HexBytes
 from pydantic import BaseModel, Field
 from web3 import HTTPProvider, Web3
@@ -47,64 +50,106 @@
 DEFAULT_PORT = 8545
 HARDHAT_CHAIN_ID = 31337
 HARDHAT_CONFIG = """
 // See https://hardhat.org/config/ for config options.
 module.exports = {{
   networks: {{
     hardhat: {{
-      hardfork: "london",
+      hardfork: "{hard_fork}",
       // Base fee of 0 allows use of 0 gas price when testing
       initialBaseFeePerGas: 0,
       accounts: {{
         mnemonic: "{mnemonic}",
-        path: "m/44'/60'/0'",
+        path: "{hd_path}",
         count: {number_of_accounts}
       }}
     }},
   }},
 }};
-"""
-HARDHAT_CONFIG_FILE_NAME = "hardhat.config.js"
+""".lstrip()
+HARDHAT_HD_PATH = "m/44'/60'/0'"
+DEFAULT_HARDHAT_CONFIG_FILE_NAME = "hardhat.config.js"
+HARDHAT_CONFIG_FILE_NAME_OPTIONS = (DEFAULT_HARDHAT_CONFIG_FILE_NAME, "hardhat.config.ts")
 HARDHAT_PLUGIN_PATTERN = re.compile(r"hardhat-[A-Za-z0-9-]+$")
+DEFAULT_HARDHAT_HARD_FORK = "shanghai"
 _NO_REASON_REVERT_MESSAGE = "Transaction reverted without a reason string"
 _REVERT_REASON_PREFIX = (
     "Error: VM Exception while processing transaction: reverted with reason string "
 )
 
 
-class HardhatConfigJS:
-    """
-    A class representing the actual ``hardhat.config.js`` file.
-    """
-
-    def __init__(
-        self,
-        project_path: Path,
-        mnemonic: str,
-        num_of_accounts: int,
-        hard_fork: Optional[str] = None,
-    ):
-        self._base_path = project_path
-        self._mnemonic = mnemonic
-        self._num_of_accounts = num_of_accounts
-        self._hard_fork = hard_fork or "london"
-
-    @property
-    def _content(self) -> str:
-        return HARDHAT_CONFIG.format(
-            mnemonic=self._mnemonic, number_of_accounts=self._num_of_accounts
+def _validate_hardhat_config_file(
+    path: Path,
+    mnemonic: str,
+    num_of_accounts: int,
+    hard_fork: str = DEFAULT_HARDHAT_HARD_FORK,
+):
+    if not path.is_file() and path.is_dir():
+        path = path / DEFAULT_HARDHAT_CONFIG_FILE_NAME
+
+    elif path.name not in HARDHAT_CONFIG_FILE_NAME_OPTIONS:
+        raise ValueError(
+            f"Expecting file name to be one of '{', '.join(HARDHAT_CONFIG_FILE_NAME_OPTIONS)}'. "
+            f"Receiver '{path.name}'."
         )
 
-    @property
-    def _path(self) -> Path:
-        return self._base_path / HARDHAT_CONFIG_FILE_NAME
+    content = HARDHAT_CONFIG.format(
+        hd_path=HARDHAT_HD_PATH,
+        mnemonic=mnemonic,
+        number_of_accounts=num_of_accounts,
+        hard_fork=hard_fork,
+    )
+    if not path.is_file():
+        # Create default '.js' file.
+        logger.debug(f"Creating file '{path.name}'.")
+        path.parent.mkdir(parents=True, exist_ok=True)
+        path.write_text(content)
+        return path
+
+    invalid_config_warning = (
+        f"Existing '{path.name}' conflicts with ape. "
+        "Some features may not work as intended. "
+        f"The default config looks like this:\n{content}\n"
+        "NOTE: You can configure the test account mnemonic "
+        "and/or number of test accounts using your `ape-config.yaml`: "
+        "https://docs.apeworx.io/ape/stable/userguides/config.html#testing"
+    )
+
+    try:
+        js_obj = {}
+        try:
+            js_obj = parse_js_object(path.read_text())
+        except Exception:
+            # Will fail if using type-script features.
+            pass
+
+        if js_obj:
+            accounts_config = js_obj.get("networks", {}).get("hardhat", {}).get("accounts", {})
+            if not accounts_config or (
+                accounts_config.get("mnemonic") != mnemonic
+                or accounts_config.get("count") != num_of_accounts
+                or accounts_config.get("path") != HARDHAT_HD_PATH
+            ):
+                logger.warning(invalid_config_warning)
 
-    def write_if_not_exists(self):
-        if not self._path.is_file():
-            self._path.write_text(self._content)
+        else:
+            # Not as good of a check, but we do our best.
+            content = path.read_text()
+            if (
+                mnemonic not in content
+                or HARDHAT_HD_PATH not in content
+                or str(num_of_accounts) not in content
+            ):
+                logger.warning(invalid_config_warning)
+
+    except Exception as err:
+        logger.error(
+            f"Failed to parse Hardhat config file: {err}. "
+            f"Some features may not work as intended."
+        )
 
 
 class PackageJson(BaseModel):
     name: Optional[str]
     version: Optional[str]
     description: Optional[str]
     dependencies: Optional[Dict[str, str]]
@@ -118,14 +163,22 @@
 
 
 class HardhatNetworkConfig(PluginConfig):
     port: Optional[Union[int, Literal["auto"]]] = DEFAULT_PORT
     request_timeout: int = 30
     fork_request_timeout: int = 300
 
+    hardhat_config_file: Optional[Path] = None
+    """
+    Optionally specify a Hardhat config file to use
+    (in the case when you don't wish to use the one Ape creates).
+    Note: If you do this, you may need to ensure its settings
+    matches Ape's.
+    """
+
     # For setting the values in --fork and --fork-block-number command arguments.
     # Used only in HardhatForkProvider.
     # Mapping of ecosystem_name => network_name => HardhatForkConfig
     fork: Dict[str, Dict[str, HardhatForkConfig]] = {}
 
     class Config:
         extra = "allow"
@@ -134,15 +187,24 @@
 def _call(*args):
     return call([*args], stderr=PIPE, stdout=PIPE, stdin=PIPE)
 
 
 class HardhatProvider(SubprocessProvider, Web3Provider, TestProviderAPI):
     port: Optional[int] = None
     attempted_ports: List[int] = []
-    unlocked_accounts: List[AddressType] = []
+
+    # Will get set to False if notices not installed correctly.
+    # However, will still attempt to connect and only raise
+    # if failed to connect. This is because sometimes Hardhat may still work,
+    # such when running via `pytester`.
+    _detected_correct_install: bool = True
+
+    @property
+    def unlocked_accounts(self) -> List[AddressType]:
+        return list(self.account_manager.test_accounts._impersonated_accounts)
 
     @property
     def mnemonic(self) -> str:
         return self._test_config.mnemonic
 
     @property
     def number_of_accounts(self) -> int:
@@ -154,34 +216,47 @@
 
     @property
     def timeout(self) -> int:
         return self.config.request_timeout
 
     @property
     def chain_id(self) -> int:
-        if hasattr(self.web3, "eth"):
-            return self.web3.eth.chain_id
-        else:
-            return HARDHAT_CHAIN_ID
+        return self.web3.eth.chain_id if hasattr(self.web3, "eth") else HARDHAT_CHAIN_ID
 
-    @cached_property
+    @property
     def npx_bin(self) -> str:
         npx = shutil.which("npx")
-
+        suffix = "See ape-hardhat README for install steps."
         if not npx:
-            raise HardhatSubprocessError(
-                "Could not locate NPM executable. See ape-hardhat README for install steps."
-            )
+            raise HardhatSubprocessError(f"Could not locate `npx` executable. {suffix}")
+
         elif _call(npx, "--version") != 0:
-            raise HardhatSubprocessError(
-                "NPM executable returned error code. See ape-hardhat README for install steps."
-            )
-        elif _call(npx, "hardhat", "--version") != 0:
+            raise HardhatSubprocessError(f"`npm` executable returned error code. {suffix}.")
+
+        # NOTE: Even if a version appears in this output, Hardhat still may not be installed
+        # because of how NPM works.
+        hardhat_version = check_output([npx, "hardhat", "--version"]).decode("utf8").strip()
+        logger.debug(f"Using Hardhat version '{hardhat_version}'.")
+        if not hardhat_version or not hardhat_version[0].isnumeric():
             raise HardhatNotInstalledError()
 
+        npm = shutil.which("npm")
+        if not npm:
+            raise HardhatSubprocessError(f"Could not locate `npm` executable. {suffix}")
+
+        try:
+            install_result = check_output([npm, "list", "hardhat", "--json"])
+        except CalledProcessError:
+            self._detected_correct_install = False
+            return npx
+
+        data = json.loads(install_result)
+
+        # This actually ensures it is installed.
+        self._detected_correct_install = "hardhat" in data.get("dependencies", {})
         return npx
 
     @property
     def project_folder(self) -> Path:
         return self.config_manager.PROJECT_FOLDER
 
     @property
@@ -199,14 +274,25 @@
         return 0
 
     @property
     def is_connected(self) -> bool:
         self._set_web3()
         return self._web3 is not None
 
+    @property
+    def hardhat_config_file(self) -> Path:
+        if self.config.hardhat_config_file and self.config.hardhat_config_file.is_dir():
+            path = self.config.hardhat_config_file / DEFAULT_HARDHAT_CONFIG_FILE_NAME
+        elif self.config.hardhat_config_file:
+            path = self.config.hardhat_config_file
+        else:
+            path = self.config_manager.DATA_FOLDER / "hardhat" / DEFAULT_HARDHAT_CONFIG_FILE_NAME
+
+        return path.expanduser().absolute()
+
     @cached_property
     def _test_config(self) -> TestConfig:
         return cast(TestConfig, self.config_manager.get_config("test"))
 
     @cached_property
     def _package_json(self) -> PackageJson:
         json_path = self.project_folder / "package.json"
@@ -235,16 +321,17 @@
         return next((True for plugin in self._hardhat_plugins if plugin == plugin_name), False)
 
     def connect(self):
         """
         Start the hardhat process and verify it's up and accepting connections.
         """
 
-        js_config = HardhatConfigJS(self.project_folder, self.mnemonic, self.number_of_accounts)
-        js_config.write_if_not_exists()
+        _validate_hardhat_config_file(
+            self.hardhat_config_file, self.mnemonic, self.number_of_accounts
+        )
 
         # NOTE: Must set port before calling 'super().connect()'.
         if not self.port:
             self.port = self.provider_settings.get("port", self.config.port)
 
         if self.is_connected:
             # Connects to already running process
@@ -275,16 +362,15 @@
                         logger.info("Retrying Hardhat subprocess startup: %r", exc)
                         self.port = None
 
     def _set_web3(self):
         if not self.port:
             return
 
-        self._web3 = Web3(HTTPProvider(self.uri, request_kwargs={"timeout": self.timeout}))
-
+        self._web3 = _create_web3(self.uri, self.timeout)
         if not self._web3.is_connected():
             self._web3 = None
             return
 
         # Verify is actually a Hardhat provider,
         # or else skip it to possibly try another port.
         client_version = self._web3.client_version.lower()
@@ -329,15 +415,21 @@
                         raise HardhatProviderError(
                             f"Unable to find an available port. Ports tried: {ports_str}"
                         )
 
                 self.port = port
 
         self.attempted_ports.append(self.port)
-        self.start()
+        try:
+            self.start()
+        except RPCTimeoutError as err:
+            if not self._detected_correct_install:
+                raise HardhatNotInstalledError() from err
+
+            raise  # RPCTimeoutError
 
     def disconnect(self):
         self._web3 = None
         self.port = None
         super().disconnect()
 
     def build_command(self) -> List[str]:
@@ -345,14 +437,16 @@
             self.npx_bin,
             "hardhat",
             "node",
             "--hostname",
             "127.0.0.1",
             "--port",
             str(self.port),
+            "--config",
+            str(self.hardhat_config_file),
         ]
 
     def set_block_gas_limit(self, gas_limit: int) -> bool:
         return self._make_request("evm_setBlockGasLimit", [hex(gas_limit)]) is True
 
     def set_code(self, address: AddressType, code: ContractCode) -> bool:
         if isinstance(code, bytes):
@@ -377,31 +471,28 @@
     def revert(self, snapshot_id: SnapshotID) -> bool:
         if isinstance(snapshot_id, int):
             snapshot_id = HexBytes(snapshot_id).hex()
 
         return self._make_request("evm_revert", [snapshot_id]) is True
 
     def unlock_account(self, address: AddressType) -> bool:
-        result = self._make_request("hardhat_impersonateAccount", [address])
-        if result:
-            self.unlocked_accounts.append(address)
-
-        return result is True
+        return self._make_request("hardhat_impersonateAccount", [address])
 
     def send_transaction(self, txn: TransactionAPI) -> ReceiptAPI:
         """
         Creates a new message call transaction or a contract creation
         for signed transactions.
         """
 
         sender = txn.sender
         if sender:
             sender = self.conversion_manager.convert(txn.sender, AddressType)
 
-        if sender in self.unlocked_accounts:
+        sender_address = cast(AddressType, sender)
+        if sender_address in self.unlocked_accounts:
             # Allow for an unsigned transaction
             txn = self.prepare_transaction(txn)
             txn_dict = txn.dict()
             if isinstance(txn_dict.get("type"), int):
                 txn_dict["type"] = HexBytes(txn_dict["type"]).hex()
 
             txn_params = cast(TxParams, txn_dict)
@@ -617,7 +708,12 @@
     def reset_fork(self, block_number: Optional[int] = None):
         forking_params: Dict[str, Union[str, int]] = {"jsonRpcUrl": self.fork_url}
         block_number = block_number if block_number is not None else self.fork_block_number
         if block_number is not None:
             forking_params["blockNumber"] = block_number
 
         return self._make_request("hardhat_reset", [{"forking": forking_params}])
+
+
+def _create_web3(uri: str, timeout: int) -> Web3:
+    # NOTE: This method exists so can be mocked in testing.
+    return Web3(HTTPProvider(uri, request_kwargs={"timeout": timeout}))
```

### Comparing `ape-hardhat-0.6.4/ape_hardhat.egg-info/PKG-INFO` & `ape-hardhat-0.6.5/ape_hardhat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-hardhat
-Version: 0.6.4
+Version: 0.6.5
 Summary: ape-hardhat: Ape network provider for Hardhat
 Home-page: https://github.com/ApeWorX/ape-hardhat
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
         
@@ -105,14 +105,27 @@
                 enable_hardhat_deployments: true
         ```
         
         ```bash
         ape plugins install alchemy
         ```
         
+        ## Custom Hardhat Config File
+        
+        By default, Ape generates and uses a basic config file for starting up a Hardhat node and having the same test accounts that Ape expects.
+        To avoid conflict with other pre-existing Hardhat config files, Ape generates one in `$HOME/.ape/hardhat` and always refers to that one.
+        To use a different one, such as the one in your local project instead, add the following to your `ape-config.yaml`:
+        
+        ```yaml
+        hardhat:
+          hardhat_config_file: ./hardhat.config.ts
+        ```
+        
+        **NOTE**: You can refer to either a Hardhat JS file or a Hardhat TS file.
+        
         ## Development
         
         Please see the [contributing guide](CONTRIBUTING.md) to learn more how to contribute to this project.
         Comments, questions, criticisms and pull requests are welcomed.
         
 Keywords: ethereum
 Platform: UNKNOWN
```

### Comparing `ape-hardhat-0.6.4/ape_hardhat.egg-info/SOURCES.txt` & `ape-hardhat-0.6.5/ape_hardhat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 tests/test_gas_report.py
 tests/test_provider.py
 tests/test_trace.py
 tests/data/contracts/ethereum/local/contract_a.json
 tests/data/contracts/ethereum/local/contract_b.json
 tests/data/contracts/ethereum/local/contract_c.json
 tests/data/contracts/ethereum/local/has_error.json
+tests/data/contracts/ethereum/local/reverts_contract.json
 tests/data/contracts/ethereum/local/solidity_contract.json
+tests/data/contracts/ethereum/local/sub_reverts_contract.json
 tests/data/contracts/ethereum/local/token_a.json
 tests/data/contracts/ethereum/local/token_b.json
 tests/data/contracts/ethereum/local/vyper_contract.json
 tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
 tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
 tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
 tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
@@ -107,9 +109,12 @@
 tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
 tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
 tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
 tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
 tests/data/python/pytest_test_conftest.py
 tests/data/python/pytest_tests.py
 tests/data/sources/HasError.sol
+tests/data/sources/RevertsContractVy.vy
+tests/data/sources/SubRevertsVy.vy
 tests/data/sources/TokenA.vy
-tests/data/sources/TokenB.vy
+tests/data/sources/TokenB.vy
+tests/data/sources/interfaces/ISubRevertsVy.vy
```

### Comparing `ape-hardhat-0.6.4/ape_hardhat.egg-info/requires.txt` & `ape-hardhat-0.6.5/ape_hardhat.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-eth-ape<0.7,>=0.6.8
+eth-ape<0.7,>=0.6.9
 evm-trace
 hexbytes
 web3
+chompjs<2,>=1.1.9
 
 [dev]
 pytest>=6.0
 pytest-mock
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
```

### Comparing `ape-hardhat-0.6.4/pyproject.toml` & `ape-hardhat-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/setup.py` & `ape-hardhat-0.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,19 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-hardhat",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.6.8,<0.7",
+        "eth-ape>=0.6.9,<0.7",
         "evm-trace",  # Use same version as eth-ape
         "hexbytes",  # Use same version as eth-ape
         "web3",  # Use same version as eth-ape
+        "chompjs>=1.1.9,<2",  # To help parse hardhat files
     ],
     python_requires=">=3.8,<3.11",
     extras_require=extras_require,
     py_modules=["ape_hardhat"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
```

### Comparing `ape-hardhat-0.6.4/tests/ape-config.yaml` & `ape-hardhat-0.6.5/tests/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/conftest.py` & `ape-hardhat-0.6.5/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import subprocess
 import tempfile
 from contextlib import contextmanager
 from pathlib import Path
 from tempfile import mkdtemp
 from typing import Dict, Optional
 
 import ape
@@ -13,17 +14,19 @@
 from ape.exceptions import APINotImplementedError, UnknownSnapshotError
 from ape.managers.config import CONFIG_FILE_NAME
 from ethpm_types import ContractType
 
 from ape_hardhat import HardhatProvider
 
 # NOTE: Ensure that we don't use local paths for the DATA FOLDER
-ape.config.DATA_FOLDER = Path(mkdtemp()).resolve()
+DATA_FOLDER = Path(mkdtemp()).resolve()
+ape.config.DATA_FOLDER = DATA_FOLDER
 
 BASE_CONTRACTS_PATH = Path(__file__).parent / "data" / "contracts"
+LOCAL_CONTRACTS_PATH = BASE_CONTRACTS_PATH / "ethereum" / "local"
 NAME = "hardhat"
 
 # Needed to test tracing support in core `ape test` command.
 pytest_plugins = ["pytester"]
 MAINNET_FORK_PORT = 9001
 GOERLI_FORK_PORT = 9002
 
@@ -38,14 +41,19 @@
 
 
 @pytest.fixture(scope="session")
 def name():
     return NAME
 
 
+@pytest.fixture(scope="session")
+def data_folder():
+    return DATA_FOLDER
+
+
 @pytest.fixture(scope="session", autouse=True)
 def in_tests_dir(config):
     with config.using_project(Path(__file__).parent):
         yield
 
 
 @contextmanager
@@ -115,31 +123,40 @@
 def contract_type(request, get_contract_type) -> ContractType:
     return get_contract_type(f"{request.param}_contract")
 
 
 @pytest.fixture
 def get_contract_type():
     def fn(name: str):
-        path = BASE_CONTRACTS_PATH / "ethereum" / "local" / f"{name}.json"
-        content = path.read_text()
-        return ContractType.parse_raw(content)
+        return ContractType.parse_file(LOCAL_CONTRACTS_PATH / f"{name}.json")
 
     return fn
 
 
 @pytest.fixture
 def contract_container(contract_type) -> ContractContainer:
     return ContractContainer(contract_type=contract_type)
 
 
 @pytest.fixture
 def contract_instance(owner, contract_container, connected_provider):
     return owner.deploy(contract_container)
 
 
+@pytest.fixture
+def error_contract_container(get_contract_type):
+    ct = get_contract_type("has_error")
+    return ContractContainer(ct)
+
+
+@pytest.fixture
+def error_contract(owner, error_contract_container):
+    return owner.deploy(error_contract_container)
+
+
 @pytest.fixture(scope="session")
 def sender(accounts):
     return accounts[0]
 
 
 @pytest.fixture(scope="session")
 def receiver(accounts):
@@ -148,14 +165,19 @@
 
 @pytest.fixture(scope="session")
 def owner(accounts):
     return accounts[2]
 
 
 @pytest.fixture(scope="session")
+def not_owner(accounts):
+    return accounts[3]
+
+
+@pytest.fixture(scope="session")
 def local_network_api(networks):
     return networks.ethereum.local
 
 
 @pytest.fixture
 def connected_provider(name, networks, local_network_api):
     with networks.ethereum.local.use_provider(name) as provider:
@@ -219,7 +241,44 @@
             with config.using_project(temp_dir):
                 yield temp_dir
 
             config_file.unlink()
             config._cached_configs = {}
 
     return func
+
+
+@pytest.fixture
+def contract_a(owner, connected_provider, get_contract_type):
+    contract_c = owner.deploy(ContractContainer(get_contract_type("contract_c")))
+    contract_b = owner.deploy(
+        ContractContainer(get_contract_type("contract_b")), contract_c.address
+    )
+    contract_a = owner.deploy(
+        ContractContainer(get_contract_type("contract_a")), contract_b.address, contract_c.address
+    )
+    return contract_a
+
+
+@pytest.fixture
+def mock_web3(mocker):
+    mock = mocker.MagicMock()
+    factory = mocker.patch("ape_hardhat.provider._create_web3")
+    factory.return_value = mock
+    return mock
+
+
+@pytest.fixture
+def install_detection_fail(mocker):
+    cmd = ["list", "hardhat", "--json"]
+
+    def side_effect(cmd_ls):
+        if cmd_ls[1:] == cmd:
+            # mock
+            raise subprocess.CalledProcessError(1, cmd)
+
+        # Run normally.
+        return subprocess.check_output(cmd_ls)
+
+    check_output_mock = mocker.patch("ape_hardhat.provider.check_output")
+    check_output_mock.side_effect = side_effect
+    return check_output_mock
```

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/contract_a.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/contract_a.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/contract_b.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/contract_b.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/contract_c.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/contract_c.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/has_error.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/has_error.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/solidity_contract.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/solidity_contract.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/token_a.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/token_a.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/token_b.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/token_b.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/local/vyper_contract.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/local/vyper_contract.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json` & `ape-hardhat-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/python/pytest_tests.py` & `ape-hardhat-0.6.5/tests/data/python/pytest_tests.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/sources/TokenA.vy` & `ape-hardhat-0.6.5/tests/data/sources/TokenA.vy`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/data/sources/TokenB.vy` & `ape-hardhat-0.6.5/tests/data/sources/TokenB.vy`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/expected_traces.py` & `ape-hardhat-0.6.5/tests/expected_traces.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/test_fork_provider.py` & `ape-hardhat-0.6.5/tests/test_fork_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
 
 @pytest.mark.fork
 def test_reset_fork_specify_block_number_via_config(mainnet_fork_provider):
     mainnet_fork_provider.mine(5)
     mainnet_fork_provider.reset_fork()
     block_num_after_reset = mainnet_fork_provider.get_block("latest").number
-    assert block_num_after_reset == 15776634  # Specified in ape-config.yaml
+    assert block_num_after_reset == 17040366  # Specified in ape-config.yaml
 
 
 @pytest.mark.fork
 def test_transaction(owner, mainnet_fork_contract_instance):
     receipt = mainnet_fork_contract_instance.setNumber(6, sender=owner)
     assert receipt.sender == owner
 
@@ -183,14 +183,15 @@
     networks,
     port,
     upstream_network,
     enable_hardhat_deployments,
     fork_block_number,
     has_hardhat_deploy,
     name,
+    data_folder,
 ):
     eth_config = {
         name: {
             "fork": {
                 "ethereum": {
                     upstream_network: {
                         "enable_hardhat_deployments": enable_hardhat_deployments,
@@ -200,15 +201,15 @@
             },
         },
     }
     package_json = {
         "name": "contracts",
         "version": "0.1.0",
         "dependencies": {
-            "hardhat": "^2.6.4",
+            "hardhat": "^2.13.1",
             "hardhat-ethers": "^2.0.2",
         },
     }
 
     if has_hardhat_deploy:
         package_json["devDependencies"] = {"hardhat-deploy": "^0.8.10"}
 
@@ -218,32 +219,34 @@
             name=name,
             network=network_api,
             request_header={},
             data_folder=Path("."),
             provider_settings={},
         )
         provider.port = port
-        cmd = " ".join(provider.build_command())
-        expected_cmd = [
-            provider.npx_bin,
+        actual = provider.build_command()
+        expected = [
             name,
             "node",
             "--hostname",
             "127.0.0.1",
             "--port",
             str(port),
+            "--config",
+            str(data_folder / "hardhat" / "hardhat.config.js"),
             "--fork",
             provider.fork_url,
         ]
         if not enable_hardhat_deployments and has_hardhat_deploy:
-            expected_cmd.append("--no-deploy")
+            expected.append("--no-deploy")
         if fork_block_number:
-            expected_cmd.extend(("--fork-block-number", str(fork_block_number)))
+            expected.extend(("--fork-block-number", str(fork_block_number)))
 
-        assert cmd == " ".join(expected_cmd)
+        assert actual[0].endswith("npx")
+        assert actual[1:] == expected
 
 
 @pytest.mark.fork
 def test_connect_to_polygon(networks, owner, contract_container):
     """
     Ensures we don't get PoA middleware issue.
     """
```

### Comparing `ape-hardhat-0.6.4/tests/test_gas_report.py` & `ape-hardhat-0.6.5/tests/test_gas_report.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.4/tests/test_trace.py` & `ape-hardhat-0.6.5/tests/test_trace.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import re
 import shutil
 import tempfile
 from pathlib import Path
 from typing import List
 
 import pytest
-from ape.contracts import ContractContainer
-from ethpm_types import ContractType
 
 from .expected_traces import (
     LOCAL_GAS_REPORT,
     LOCAL_TRACE,
     MAINNET_FAIL_TRACE_FIRST_10_LINES,
     MAINNET_FAIL_TRACE_LAST_10_LINES,
     MAINNET_TRACE_FIRST_10_LINES,
@@ -52,30 +50,14 @@
     params=(MAINNET_TXN_HASH, MAINNET_FAIL_TXN_HASH),
 )
 def mainnet_receipt(request, mainnet_fork_provider):
     return mainnet_fork_provider.get_receipt(request.param)
 
 
 @pytest.fixture
-def contract_a(owner, connected_provider):
-    base_path = BASE_CONTRACTS_PATH / "local"
-
-    def get_contract_type(suffix: str) -> ContractType:
-        return ContractType.parse_file(base_path / f"contract_{suffix}.json")
-
-    contract_c = owner.deploy(ContractContainer(get_contract_type("c")))
-    contract_b = owner.deploy(ContractContainer(get_contract_type("b")), contract_c.address)
-    contract_a = owner.deploy(
-        ContractContainer(get_contract_type("a")), contract_b.address, contract_c.address
-    )
-
-    return contract_a
-
-
-@pytest.fixture
 def local_receipt(contract_a, owner):
     return contract_a.methodWithoutArguments(sender=owner)
 
 
 @pytest.mark.fork
 def test_local_transaction_traces(local_receipt, captrace):
     # NOTE: Strange bug in Rich where we can't use sys.stdout for testing tree output.
```

