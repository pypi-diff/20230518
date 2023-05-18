# Comparing `tmp/holisticai-0.3.0.tar.gz` & `tmp/holisticai-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holisticai-0.3.0.tar", max compression
+gzip compressed data, was "holisticai-0.4.0.tar", max compression
```

## Comparing `holisticai-0.3.0.tar` & `holisticai-0.4.0.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0    11357 2023-01-27 14:36:29.884265 holisticai-0.3.0/LICENSE
--rw-r--r--   0        0        0      796 2023-01-27 14:36:29.884265 holisticai-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/__init__.py
--rw-r--r--   0        0        0      159 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/__init__.py
--rw-r--r--   0        0        0     3280 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/metrics/__init__.py
--rw-r--r--   0        0        0    27392 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/metrics/_classification.py
--rw-r--r--   0        0        0    20317 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/metrics/_clustering.py
--rw-r--r--   0        0        0    27996 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/metrics/_multiclass.py
--rw-r--r--   0        0        0    41982 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/metrics/_recommender.py
--rw-r--r--   0        0        0    28639 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/metrics/_regression.py
--rw-r--r--   0        0        0     2212 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/__init__.py
--rw-r--r--   0        0        0     5662 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_feature.py
--rw-r--r--   0        0        0    10434 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_repairer.py
--rw-r--r--   0        0        0     2149 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_numerical_repairer.py
--rw-r--r--   0        0        0     1365 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_sparse_list.py
--rw-r--r--   0        0        0     7801 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_utils.py
--rw-r--r--   0        0        0     2166 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/_utils.py
--rw-r--r--   0        0        0     1977 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kcenters.py
--rw-r--r--   0        0        0    14757 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kmedoids.py
--rw-r--r--   0        0        0       63 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_base.py
--rw-r--r--   0        0        0     8244 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_scalable.py
--rw-r--r--   0        0        0     2832 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_vanilla.py
--rw-r--r--   0        0        0      140 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/__init__.py
--rw-r--r--   0        0        0       63 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_base.py
--rw-r--r--   0        0        0     8117 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_scalable.py
--rw-r--r--   0        0        0     3093 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_vanilla.py
--rw-r--r--   0        0        0     1487 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/__init__.py
--rw-r--r--   0        0        0      740 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/dataset.py
--rw-r--r--   0        0        0     2088 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/models.py
--rw-r--r--   0        0        0     6067 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/trainer.py
--rw-r--r--   0        0        0     7278 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/transformer.py
--rw-r--r--   0        0        0       66 2023-01-27 14:36:29.936265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/commons/__init__.py
--rw-r--r--   0        0        0      475 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/commons/_conventions.py
--rw-r--r--   0        0        0     2381 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/commons/_logger.py
--rw-r--r--   0        0        0     2225 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/commons/_moments_utils.py
--rw-r--r--   0        0        0    10220 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/commons/classification/_constraints.py
--rw-r--r--   0        0        0      906 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/commons/classification/_objectives.py
--rw-r--r--   0        0        0     4382 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/commons/regression/_constraints.py
--rw-r--r--   0        0        0     1435 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/commons/regression/_losses.py
--rw-r--r--   0        0        0     7834 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/_lagrangian.py
--rw-r--r--   0        0        0     9599 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/algorithm.py
--rw-r--r--   0        0        0     6996 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/transformer.py
--rw-r--r--   0        0        0    13843 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/algorithms.py
--rw-r--r--   0        0        0     4040 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/transformer.py
--rw-r--r--   0        0        0     5017 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/algorithm.py
--rw-r--r--   0        0        0     2821 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/transformer.py
--rw-r--r--   0        0        0    11078 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/algorithm.py
--rw-r--r--   0        0        0     3473 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/transformer.py
--rw-r--r--   0        0        0     5213 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/utils.py
--rw-r--r--   0        0        0     1680 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/algorithm.py
--rw-r--r--   0        0        0     4772 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/transformer.py
--rw-r--r--   0        0        0     3582 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/grid_search/_grid_generator.py
--rw-r--r--   0        0        0     5595 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/grid_search/algorithm.py
--rw-r--r--   0        0        0     6894 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/grid_search/transformer.py
--rw-r--r--   0        0        0     3231 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/blind_spot_aware.py
--rw-r--r--   0        0        0      559 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/propensity_utils.py
--rw-r--r--   0        0        0     1853 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/utils.py
--rw-r--r--   0        0        0     3541 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm.py
--rw-r--r--   0        0        0     9446 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm_utils.py
--rw-r--r--   0        0        0     4496 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/transformer.py
--rw-r--r--   0        0        0     2950 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/popularity_propensity.py
--rw-r--r--   0        0        0     5282 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm.py
--rw-r--r--   0        0        0      614 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm_utils.py
--rw-r--r--   0        0        0     3432 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/constraints.py
--rw-r--r--   0        0        0     3952 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/transformer.py
--rw-r--r--   0        0        0     3456 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm.py
--rw-r--r--   0        0        0     3437 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm_utils.py
--rw-r--r--   0        0        0     3884 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/losses.py
--rw-r--r--   0        0        0     4097 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/model.py
--rw-r--r--   0        0        0     6557 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/transformer.py
--rw-r--r--   0        0        0     2217 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/algorithm.py
--rw-r--r--   0        0        0     2254 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/transformer.py
--rw-r--r--   0        0        0     2231 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm.py
--rw-r--r--   0        0        0     2097 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_bound_update.py
--rw-r--r--   0        0        0     5463 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_fair_clustering.py
--rw-r--r--   0        0        0      828 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_logger.py
--rw-r--r--   0        0        0     4915 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_method_utils.py
--rw-r--r--   0        0        0     3457 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_methods.py
--rw-r--r--   0        0        0     3104 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_utils.py
--rw-r--r--   0        0        0     4959 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/transformer.py
--rw-r--r--   0        0        0     1165 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/__init__.py
--rw-r--r--   0        0        0     8950 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/calibrated_eq_odds_postprocessing.py
--rw-r--r--   0        0        0     9796 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm.py
--rw-r--r--   0        0        0     7433 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm_utils.py
--rw-r--r--   0        0        0     6954 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/transformer.py
--rw-r--r--   0        0        0     4006 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/disparate_impact_remover_rs.py
--rw-r--r--   0        0        0     9231 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/eq_odds_postprocessing.py
--rw-r--r--   0        0        0     6784 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/fail_prob.py
--rw-r--r--   0        0        0     1963 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/mtable_generator.py
--rw-r--r--   0        0        0     2220 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/valitation_utils.py
--rw-r--r--   0        0        0     7114 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/fair_topk/transformer.py
--rw-r--r--   0        0        0     3690 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm.py
--rw-r--r--   0        0        0     2278 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm_utils.py
--rw-r--r--   0        0        0     2481 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/constraints.py
--rw-r--r--   0        0        0     6238 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/transformer.py
--rw-r--r--   0        0        0     3712 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm.py
--rw-r--r--   0        0        0      868 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm_utils.py
--rw-r--r--   0        0        0     6369 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/constraints.py
--rw-r--r--   0        0        0     5421 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/transformer.py
--rw-r--r--   0        0        0     4286 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/algorithm.py
--rw-r--r--   0        0        0     3570 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/transformer.py
--rw-r--r--   0        0        0     4032 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm.py
--rw-r--r--   0        0        0     1668 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm_utils.py
--rw-r--r--   0        0        0     5413 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm.py
--rw-r--r--   0        0        0     2791 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm_utils.py
--rw-r--r--   0        0        0     4968 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm.py
--rw-r--r--   0        0        0      640 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm_utils.py
--rw-r--r--   0        0        0     5751 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/transformer.py
--rw-r--r--   0        0        0     1314 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm.py
--rw-r--r--   0        0        0     1294 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm_utils.py
--rw-r--r--   0        0        0     3688 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/transformer.py
--rw-r--r--   0        0        0    10585 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/reject_option_classification.py
--rw-r--r--   0        0        0     2177 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/algorithm.py
--rw-r--r--   0        0        0     3599 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/transformer.py
--rw-r--r--   0        0        0      578 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/preprocessing/__init__.py
--rw-r--r--   0        0        0     3891 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/preprocessing/correlation_remover.py
--rw-r--r--   0        0        0     2638 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/preprocessing/disparate_impact_remover.py
--rw-r--r--   0        0        0     3833 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/preprocessing/fairlet_clustering/transformer.py
--rw-r--r--   0        0        0     7337 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/preprocessing/learning_fair_representation.py
--rw-r--r--   0        0        0     3813 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/mitigation/preprocessing/reweighing.py
--rw-r--r--   0        0        0     1266 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/plots/__init__.py
--rw-r--r--   0        0        0     2157 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/plots/_bias_classification_plots.py
--rw-r--r--   0        0        0     6909 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/plots/_bias_exploratory_plots.py
--rw-r--r--   0        0        0    11183 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/plots/_bias_multiclass_plots.py
--rw-r--r--   0        0        0     8066 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/plots/_bias_recommender_plots.py
--rw-r--r--   0        0        0    14148 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/bias/plots/_bias_regression_plots.py
--rw-r--r--   0        0        0      333 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/datasets/__init__.py
--rw-r--r--   0        0        0    13961 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/datasets/_dataloaders.py
--rw-r--r--   0        0        0      951 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/datasets/synthetic/recruitment.py
--rw-r--r--   0        0        0      966 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/datasets/synthetic/user_feedback.py
--rw-r--r--   0        0        0       54 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/pipeline/__init__.py
--rw-r--r--   0        0        0     5952 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/pipeline/_pipeline.py
--rw-r--r--   0        0        0     6559 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/pipeline/_pipeline_helper.py
--rw-r--r--   0        0        0     3134 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/pipeline/handlers/_estimator.py
--rw-r--r--   0        0        0     1821 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/pipeline/handlers/_pipeline_params.py
--rw-r--r--   0        0        0     4816 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/pipeline/handlers/_utransformers.py
--rw-r--r--   0        0        0      435 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/__init__.py
--rw-r--r--   0        0        0     5103 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/_formatting.py
--rw-r--r--   0        0        0     1353 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/_plotting.py
--rw-r--r--   0        0        0     5755 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/_recommender_tools.py
--rw-r--r--   0        0        0    13794 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/_validation.py
--rw-r--r--   0        0        0      100 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/models/cluster/__init__.py
--rw-r--r--   0        0        0     1908 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/models/cluster/_kcenters.py
--rw-r--r--   0        0        0    14757 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/models/cluster/_kmedoids.py
--rw-r--r--   0        0        0      549 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/models/cluster/_utils.py
--rw-r--r--   0        0        0      813 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/models/recommender/_rsbase.py
--rw-r--r--   0        0        0     3157 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/models/recommender/item_selection/selectors.py
--rw-r--r--   0        0        0     1321 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/models/recommender/matrix_factorization/non_negative.py
--rw-r--r--   0        0        0       68 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/optimizers/__init__.py
--rw-r--r--   0        0        0    15852 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/optimizers/_genetic_algorithm.py
--rw-r--r--   0        0        0     4484 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/transformers/_transformer_base.py
--rw-r--r--   0        0        0      499 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/transformers/bias/__init__.py
--rw-r--r--   0        0        0     1049 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/transformers/bias/_group_utils.py
--rw-r--r--   0        0        0     1243 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/transformers/bias/_inprocessing.py
--rw-r--r--   0        0        0     2137 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/transformers/bias/_postprocessing.py
--rw-r--r--   0        0        0     1346 2023-01-27 14:36:29.940265 holisticai-0.3.0/holisticai/utils/transformers/bias/_preprocessing.py
--rw-r--r--   0        0        0      698 2023-01-27 14:36:37.084217 holisticai-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4674 1970-01-01 00:00:00.000000 holisticai-0.3.0/setup.py
--rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 holisticai-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-18 12:20:34.013740 holisticai-0.4.0/LICENSE
+-rw-r--r--   0        0        0      796 2023-05-18 12:20:34.013740 holisticai-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 12:20:34.077741 holisticai-0.4.0/holisticai/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-18 12:20:34.077741 holisticai-0.4.0/holisticai/bias/__init__.py
+-rw-r--r--   0        0        0     3378 2023-05-18 12:20:34.077741 holisticai-0.4.0/holisticai/bias/metrics/__init__.py
+-rw-r--r--   0        0        0    28027 2023-05-18 12:20:34.077741 holisticai-0.4.0/holisticai/bias/metrics/_classification.py
+-rw-r--r--   0        0        0    20317 2023-05-18 12:20:34.077741 holisticai-0.4.0/holisticai/bias/metrics/_clustering.py
+-rw-r--r--   0        0        0    27996 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/metrics/_multiclass.py
+-rw-r--r--   0        0        0    41982 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/metrics/_recommender.py
+-rw-r--r--   0        0        0    30079 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/metrics/_regression.py
+-rw-r--r--   0        0        0     2212 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/__init__.py
+-rw-r--r--   0        0        0     5662 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_feature.py
+-rw-r--r--   0        0        0    10434 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_repairer.py
+-rw-r--r--   0        0        0     2149 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_numerical_repairer.py
+-rw-r--r--   0        0        0     1365 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_sparse_list.py
+-rw-r--r--   0        0        0     7801 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_utils.py
+-rw-r--r--   0        0        0     2166 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/_utils.py
+-rw-r--r--   0        0        0     1977 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kcenters.py
+-rw-r--r--   0        0        0    14757 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kmedoids.py
+-rw-r--r--   0        0        0       63 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_base.py
+-rw-r--r--   0        0        0     8244 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_scalable.py
+-rw-r--r--   0        0        0     2832 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_vanilla.py
+-rw-r--r--   0        0        0      140 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_base.py
+-rw-r--r--   0        0        0     8117 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_scalable.py
+-rw-r--r--   0        0        0     3093 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_vanilla.py
+-rw-r--r--   0        0        0     1487 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/__init__.py
+-rw-r--r--   0        0        0      740 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/dataset.py
+-rw-r--r--   0        0        0     2088 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/models.py
+-rw-r--r--   0        0        0     6067 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/trainer.py
+-rw-r--r--   0        0        0     7278 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/transformer.py
+-rw-r--r--   0        0        0       66 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/__init__.py
+-rw-r--r--   0        0        0      475 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/_conventions.py
+-rw-r--r--   0        0        0     2381 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/_logger.py
+-rw-r--r--   0        0        0     2225 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/_moments_utils.py
+-rw-r--r--   0        0        0    10220 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/classification/_constraints.py
+-rw-r--r--   0        0        0      906 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/classification/_objectives.py
+-rw-r--r--   0        0        0     4382 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/regression/_constraints.py
+-rw-r--r--   0        0        0     1435 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/regression/_losses.py
+-rw-r--r--   0        0        0     7834 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/_lagrangian.py
+-rw-r--r--   0        0        0     9599 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/algorithm.py
+-rw-r--r--   0        0        0     6923 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/transformer.py
+-rw-r--r--   0        0        0    13843 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/algorithms.py
+-rw-r--r--   0        0        0     4152 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/transformer.py
+-rw-r--r--   0        0        0     5017 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/algorithm.py
+-rw-r--r--   0        0        0     2821 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/transformer.py
+-rw-r--r--   0        0        0    11078 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/algorithm.py
+-rw-r--r--   0        0        0     3473 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/transformer.py
+-rw-r--r--   0        0        0     5213 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/utils.py
+-rw-r--r--   0        0        0     1680 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/algorithm.py
+-rw-r--r--   0        0        0     4772 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/transformer.py
+-rw-r--r--   0        0        0     3341 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/grid_search/_grid_generator.py
+-rw-r--r--   0        0        0     5623 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/grid_search/algorithm.py
+-rw-r--r--   0        0        0     6894 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/grid_search/transformer.py
+-rw-r--r--   0        0        0     3231 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/blind_spot_aware.py
+-rw-r--r--   0        0        0      559 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/propensity_utils.py
+-rw-r--r--   0        0        0     1853 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/utils.py
+-rw-r--r--   0        0        0     3541 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm.py
+-rw-r--r--   0        0        0     9446 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm_utils.py
+-rw-r--r--   0        0        0     4496 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/transformer.py
+-rw-r--r--   0        0        0     2950 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/popularity_propensity.py
+-rw-r--r--   0        0        0     5282 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm.py
+-rw-r--r--   0        0        0      614 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm_utils.py
+-rw-r--r--   0        0        0     3432 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/constraints.py
+-rw-r--r--   0        0        0     3952 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/transformer.py
+-rw-r--r--   0        0        0     3456 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm.py
+-rw-r--r--   0        0        0     3437 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm_utils.py
+-rw-r--r--   0        0        0     3884 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/losses.py
+-rw-r--r--   0        0        0     4097 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/model.py
+-rw-r--r--   0        0        0     6557 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/transformer.py
+-rw-r--r--   0        0        0     2217 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/algorithm.py
+-rw-r--r--   0        0        0     2254 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/transformer.py
+-rw-r--r--   0        0        0     2231 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm.py
+-rw-r--r--   0        0        0     2097 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_bound_update.py
+-rw-r--r--   0        0        0     5463 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_fair_clustering.py
+-rw-r--r--   0        0        0      828 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_logger.py
+-rw-r--r--   0        0        0     4915 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_method_utils.py
+-rw-r--r--   0        0        0     3457 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_methods.py
+-rw-r--r--   0        0        0     3104 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_utils.py
+-rw-r--r--   0        0        0     4954 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/transformer.py
+-rw-r--r--   0        0        0     1223 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/__init__.py
+-rw-r--r--   0        0        0     8950 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/calibrated_eq_odds_postprocessing.py
+-rw-r--r--   0        0        0     9796 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm.py
+-rw-r--r--   0        0        0     7433 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm_utils.py
+-rw-r--r--   0        0        0     6954 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/transformer.py
+-rw-r--r--   0        0        0     4006 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/disparate_impact_remover_rs.py
+-rw-r--r--   0        0        0     9322 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/eq_odds_postprocessing.py
+-rw-r--r--   0        0        0     6784 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/fail_prob.py
+-rw-r--r--   0        0        0     1963 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/mtable_generator.py
+-rw-r--r--   0        0        0     2220 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/valitation_utils.py
+-rw-r--r--   0        0        0     7114 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/transformer.py
+-rw-r--r--   0        0        0     3690 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm.py
+-rw-r--r--   0        0        0     2278 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm_utils.py
+-rw-r--r--   0        0        0     2481 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/constraints.py
+-rw-r--r--   0        0        0     6238 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/transformer.py
+-rw-r--r--   0        0        0     3712 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm.py
+-rw-r--r--   0        0        0      868 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm_utils.py
+-rw-r--r--   0        0        0     6369 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/constraints.py
+-rw-r--r--   0        0        0     5421 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/transformer.py
+-rw-r--r--   0        0        0     4286 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/algorithm.py
+-rw-r--r--   0        0        0     3570 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/transformer.py
+-rw-r--r--   0        0        0     4032 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm.py
+-rw-r--r--   0        0        0     1668 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm_utils.py
+-rw-r--r--   0        0        0     5413 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm.py
+-rw-r--r--   0        0        0     2791 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm_utils.py
+-rw-r--r--   0        0        0     4968 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm.py
+-rw-r--r--   0        0        0      640 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm_utils.py
+-rw-r--r--   0        0        0     5751 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/transformer.py
+-rw-r--r--   0        0        0     1314 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm.py
+-rw-r--r--   0        0        0     1294 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm_utils.py
+-rw-r--r--   0        0        0     3688 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/transformer.py
+-rw-r--r--   0        0        0    10585 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/reject_option_classification.py
+-rw-r--r--   0        0        0     2177 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/algorithm.py
+-rw-r--r--   0        0        0     3599 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/transformer.py
+-rw-r--r--   0        0        0      578 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3873 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/correlation_remover.py
+-rw-r--r--   0        0        0     2674 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/disparate_impact_remover.py
+-rw-r--r--   0        0        0     3914 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/fairlet_clustering/transformer.py
+-rw-r--r--   0        0        0     7337 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/learning_fair_representation.py
+-rw-r--r--   0        0        0     3813 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/reweighing.py
+-rw-r--r--   0        0        0     1266 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/plots/__init__.py
+-rw-r--r--   0        0        0     2157 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/plots/_bias_classification_plots.py
+-rw-r--r--   0        0        0     6909 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/plots/_bias_exploratory_plots.py
+-rw-r--r--   0        0        0    11349 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/plots/_bias_multiclass_plots.py
+-rw-r--r--   0        0        0     8066 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/plots/_bias_recommender_plots.py
+-rw-r--r--   0        0        0    14148 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/plots/_bias_regression_plots.py
+-rw-r--r--   0        0        0      333 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/datasets/__init__.py
+-rw-r--r--   0        0        0    13961 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/datasets/_dataloaders.py
+-rw-r--r--   0        0        0      951 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/datasets/synthetic/recruitment.py
+-rw-r--r--   0        0        0      966 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/datasets/synthetic/user_feedback.py
+-rw-r--r--   0        0        0    11570 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/efficacy/metrics.py
+-rw-r--r--   0        0        0       54 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/pipeline/__init__.py
+-rw-r--r--   0        0        0     5952 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/pipeline/_pipeline.py
+-rw-r--r--   0        0        0     6559 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/pipeline/_pipeline_helper.py
+-rw-r--r--   0        0        0     3134 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/pipeline/handlers/_estimator.py
+-rw-r--r--   0        0        0     1821 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/pipeline/handlers/_pipeline_params.py
+-rw-r--r--   0        0        0     4816 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/pipeline/handlers/_utransformers.py
+-rw-r--r--   0        0        0      435 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/__init__.py
+-rw-r--r--   0        0        0     5103 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/_formatting.py
+-rw-r--r--   0        0        0     1353 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/_plotting.py
+-rw-r--r--   0        0        0     5755 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/_recommender_tools.py
+-rw-r--r--   0        0        0    13794 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/_validation.py
+-rw-r--r--   0        0        0      100 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/models/cluster/__init__.py
+-rw-r--r--   0        0        0     1908 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/models/cluster/_kcenters.py
+-rw-r--r--   0        0        0    14757 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/models/cluster/_kmedoids.py
+-rw-r--r--   0        0        0      549 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/models/cluster/_utils.py
+-rw-r--r--   0        0        0      813 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/models/recommender/_rsbase.py
+-rw-r--r--   0        0        0     3157 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/models/recommender/item_selection/selectors.py
+-rw-r--r--   0        0        0     1321 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/models/recommender/matrix_factorization/non_negative.py
+-rw-r--r--   0        0        0       68 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/optimizers/__init__.py
+-rw-r--r--   0        0        0    15852 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/optimizers/_genetic_algorithm.py
+-rw-r--r--   0        0        0     4484 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/transformers/_transformer_base.py
+-rw-r--r--   0        0        0      499 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/transformers/bias/__init__.py
+-rw-r--r--   0        0        0     1049 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/transformers/bias/_group_utils.py
+-rw-r--r--   0        0        0     1243 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/transformers/bias/_inprocessing.py
+-rw-r--r--   0        0        0     2137 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/transformers/bias/_postprocessing.py
+-rw-r--r--   0        0        0     1346 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/transformers/bias/_preprocessing.py
+-rw-r--r--   0        0        0      698 2023-05-18 12:20:34.085741 holisticai-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 holisticai-0.4.0/PKG-INFO
```

### Comparing `holisticai-0.3.0/LICENSE` & `holisticai-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/README.md` & `holisticai-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/metrics/__init__.py` & `holisticai-0.4.0/holisticai/bias/metrics/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     cohen_d,
     disparate_impact,
     equal_opportunity_diff,
     false_negative_rate_diff,
     false_positive_rate_diff,
     four_fifths,
     statistical_parity,
+    success_rate,
     true_negative_rate_diff,
     z_test_diff,
     z_test_ratio,
 )
 
 # Clustering
 from ._clustering import (
@@ -73,14 +74,15 @@
     mae_ratio,
     max_statistical_parity,
     no_disparate_impact_level,
     regression_bias_metrics,
     rmse_ratio,
     statistical_parity_auc,
     statistical_parity_regression,
+    success_rate_regression,
     zscore_diff,
 )
 
 # All bias functions and classes
 __all__ = [
     "statistical_parity",
     "disparate_impact",
@@ -88,14 +90,16 @@
     "cohen_d",
     "accuracy_diff",
     "false_negative_rate_diff",
     "true_negative_rate_diff",
     "abroca",
     "statistical_parity_regression",
     "disparate_impact_regression",
+    "success_rate_regression",
+    "success_rate",
     "no_disparate_impact_level",
     "avg_score_diff",
     "avg_score_ratio",
     "zscore_diff",
     "max_statistical_parity",
     "statistical_parity_auc",
     "correlation_diff",
```

### Comparing `holisticai-0.3.0/holisticai/bias/metrics/_classification.py` & `holisticai-0.4.0/holisticai/bias/metrics/_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,35 @@
     # calculate sr_a and sr_b
     sr_a = _group_success_rate(group_a, y_pred)  # success rate group_a
     sr_b = _group_success_rate(group_b, y_pred)  # success rate group_b
 
     return sr_a - sr_b
 
 
+def success_rate(group_a, group_b, y_pred):
+    """
+    Calculates the raw success rates for each group.
+    Parameters
+    ----------
+    group_a : array-like
+        Group membership vector (binary)
+    group_b : array-like
+        Group membership vector (binary)
+    y_pred : array-like
+        Predictions vector (binary)
+    Returns
+    -------
+    dict
+        Dictionary with two keys, sr_a and sr_b (success rate for group a and b)
+    """
+    sr_a = _group_success_rate(group_a, y_pred)  # success rate group_a
+    sr_b = _group_success_rate(group_b, y_pred)  # success rate group_b
+    return {"sr_a": sr_a, "sr_b": sr_b}
+
+
 def disparate_impact(group_a, group_b, y_pred):
     """
     Disparate Impact.
 
     Description
     -----------
     This function computes the disparate impact (ratio of success rates)
```

### Comparing `holisticai-0.3.0/holisticai/bias/metrics/_clustering.py` & `holisticai-0.4.0/holisticai/bias/metrics/_clustering.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/metrics/_multiclass.py` & `holisticai-0.4.0/holisticai/bias/metrics/_multiclass.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/metrics/_recommender.py` & `holisticai-0.4.0/holisticai/bias/metrics/_recommender.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/metrics/_regression.py` & `holisticai-0.4.0/holisticai/bias/metrics/_regression.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,53 @@
 import pandas as pd
 
 # utils
 from ...utils._formatting import slice_arrays_by_quantile
 from ...utils._validation import _check_non_empty, _regression_checks
 
 
+def _calc_success_rate(group_membership: np.array, threshold=float):
+    return (group_membership > threshold).mean()
+
+
+def success_rate_regression(group_a, group_b, y_pred, threshold=0.50):
+    """
+    Calculates the raw success rates for each group.
+    Parameters
+    ----------
+    group_a : array-like
+        Group membership vector (binary)
+    group_b : array-like
+        Group membership vector (binary)
+    y_pred : array-like
+        Predictions vector (numerical)
+    threshold: float, str
+        The number above which the result is considered a success. Also accepts 'median' and 'mean'.
+    Returns
+    -------
+    dict
+        Dictionary with two keys, sr_a and sr_b (success rate for group a and b)
+    """
+    # Needs to be numpy array or the following operations won't be correct
+    if (type(threshold) == str) and (threshold not in set(["median", "mean"])):
+        raise ValueError("Threshold not recognised")
+    if threshold == "median":
+        threshold = np.median(y_pred)
+    if threshold == "mean":
+        threshold = np.mean(y_pred)
+    group_a = np.array(group_a)
+    group_b = np.array(group_b)
+    y_pred = np.array(y_pred)
+    group_a_membership = y_pred[group_a == 1]
+    group_b_membership = y_pred[group_b == 1]
+    sr_a = _calc_success_rate(group_a_membership, threshold)
+    sr_b = _calc_success_rate(group_b_membership, threshold)  # success rate group_b
+    return {"sr_a": sr_a, "sr_b": sr_b}
+
+
 def disparate_impact_regression(group_a, group_b, y_pred, q=0.8):
     r"""
     Disparate Impact quantile (Regression version).
 
     Description
     -----------
     This function computes the ratio of success rates between group_a and
```

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/__init__.py` & `holisticai-0.4.0/holisticai/bias/mitigation/__init__.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_feature.py` & `holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_feature.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_repairer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_repairer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_numerical_repairer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_numerical_repairer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_sparse_list.py` & `holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_sparse_list.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kcenters.py` & `holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kcenters.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kmedoids.py` & `holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kmedoids.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_scalable.py` & `holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_scalable.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_vanilla.py` & `holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_vanilla.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_scalable.py` & `holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_scalable.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_vanilla.py` & `holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_vanilla.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/__init__.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/dataset.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/dataset.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/models.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/models.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/trainer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/commons/_logger.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/_logger.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/commons/_moments_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/_moments_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/commons/classification/_constraints.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/classification/_constraints.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/commons/classification/_objectives.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/classification/_objectives.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/commons/regression/_constraints.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/regression/_constraints.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/commons/regression/_losses.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/regression/_losses.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/_lagrangian.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/_lagrangian.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,26 +40,23 @@
         nu: Optional[float] = None,
         eta0: Optional[float] = 2.0,
         loss: str = "ZeroOne",
         min_val: float = None,
         max_val: float = None,
         upper_bound: float = 0.01,
         verbose: Optional[int] = 0,
+        estimator=None,
     ):
 
         """
+
         Parameters
         ----------
-
-        estimator: An estimator implementing methods
-            ``fit(X, y, sample_weight)`` and ``predict(X)``, where ``X`` is
-            the matrix of features, ``y`` is the vector of labels, and
-            ``sample_weight`` is a vector of weights; labels ``y`` and
-            predictions returned by ``predict(X)`` are either 0 or 1 -- e.g.
-            scikit-learn classifiers.
+        estimator : sklearn-like
+            The model you want to mitigate bias for.
 
         constraints (str or BaseMoment): If string, keyword
             denoting the :class:`BaseMoment` object
             defining the disparity constraints:
             [
                 "DemographicParity",
                 "EqualizedOdds",
@@ -103,16 +100,22 @@
         self.nu = nu
         self.eta0 = eta0
         self.loss = loss
         self.min_val = min_val
         self.max_val = max_val
         self.upper_bound = upper_bound
         self.verbose = verbose
+        self.estimator = estimator
 
     def transform_estimator(self, estimator):
+
+        """
+        This method is deprecated but retained for backwards-compatibility. You should pass the estimator object directly in the constructor.
+        """
+
         self.estimator = estimator
         return self
 
     def fit(
         self,
         X: np.ndarray,
         y_true: np.ndarray,
```

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/algorithms.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/algorithms.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,7 +118,10 @@
             pairwise_distances_argmin(X, Y=self.all_centroids, metric="l1")
         ]
         self.center_groups_ = p_attr[self.all_centers]
 
     @property
     def all_centers(self):
         return np.concatenate([self.centers, self.initially_given], axis=0)
+
+    def predict(self, X):
+        return pairwise_distances(self.all_centroids, X, metric="l1").argmin(axis=0)
```

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/grid_search/_grid_generator.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/grid_search/_grid_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,29 +63,23 @@
 
         return n_units
 
     def _build_grid(self):
         """Create an integer grid"""
         max_value = self._get_true_dim()
         self.accumulator = []
-        self.entry = np.zeros(self.dim)
-        self._accumulate_integer_grid(0, max_value)
-        xs = np.array(self.accumulator)
-        xs = xs * self.grid_limit / max_value
+        while True:
+            self.entry = np.zeros(self.dim)
+            self._accumulate_integer_grid(0, max_value)
+            max_value += 1
+            if len(self.accumulator) >= self.grid_size:
+                break
 
-        """
-        min_value = 0
-        if self.neg_values:
-            max_value = (max_value - 1 + 2 - 1) // 2
-            min_value = -max_value
-        xs = [np.arange(min_value, max_value + 1) for _ in range(nb_events)]
-        xs = np.meshgrid(*xs)
-        xs = np.stack([x.reshape(-1) for x in xs], axis=1)
+        xs = np.array(self.accumulator)
         xs = xs * self.grid_limit / max_value
-        """
         return xs
 
     def _accumulate_integer_grid(self, index, max_val):
         if index == self.dim:
             self.accumulator.append(self.entry.copy())
         else:
             if (index == self.dim - 1) and (self.force_L1_norm):
```

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/grid_search/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/grid_search/algorithm.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,15 +113,14 @@
             if self.constraint.PROBLEM_TYPE == "classification":
                 y_reduction = 1 * (weights > 0)
                 weights = weights.abs()
             else:
                 y_reduction = self.constraint._y_as_series
 
             current_estimator = copy.deepcopy(self.estimator)
-
             current_estimator.fit(X, y_reduction, sample_weight=weights)
 
             predict_fn = lambda X: current_estimator.predict(X)
             objective_ = self.objective.gamma(predict_fn)[0]
             gamma_ = self.constraint.gamma(predict_fn)
 
             self.monitor.save(lambda_vec, current_estimator, objective_, gamma_)
@@ -146,14 +145,15 @@
         self.lambda_vecs_ = []
         self.objectives_ = []
         self.gammas_ = []
         self.losses = []
         self.constraint_weight = float(constraint_weight)
         self.objective_weight = 1.0 - constraint_weight
         self.verbose = verbose
+        self.total_steps = 0
         self.step = 0
 
     def loss_fct(self, objective, gamma):
         return self.objective_weight * objective + self.constraint_weight * gamma.max()
 
     def save(self, lambda_vec, current_estimator, objective, gamma):
```

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/grid_search/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/grid_search/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/blind_spot_aware.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/blind_spot_aware.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/propensity_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/propensity_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/popularity_propensity.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/popularity_propensity.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/constraints.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/constraints.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/losses.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/losses.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/model.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/model.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_bound_update.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_bound_update.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_fair_clustering.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_fair_clustering.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_logger.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_logger.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_method_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_method_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_methods.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_methods.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,26 +21,26 @@
     ----------
         Ziko, Imtiaz Masud, et al. "Variational fair clustering." Proceedings of the AAAI
         Conference on Artificial Intelligence. Vol. 35. No. 12. 2021.
     """
 
     def __init__(
         self,
-        nb_clusters: Optional[int],
+        n_clusters: Optional[int],
         lipchitz_value: Optional[str] = 1,
         lmbda: Optional[float] = 0.7,
         method: Optional[str] = "kmeans",
         normalize_input: Optional[bool] = True,
         seed: Optional[int] = None,
         verbose: Optional[int] = 0,
     ):
         """
         Parameters
         ----------
-            nb_clusters : int
+            n_clusters : int
                 The number of clusters to form as well as the number of centroids to generate.
 
             lipchitz_value : float
                 Lipchitz value in bound update
 
             lmbda : float
                 specified lambda parameter
@@ -55,23 +55,23 @@
                 Random seed.
 
             verbose : bool
                 If true , print metrics
         """
         # Constant parameters
         self.algorithm = FairClusteringAlgorithm(
-            K=nb_clusters,
+            K=n_clusters,
             L=lipchitz_value,
             lmbda=lmbda,
             method=method,
             normalize_input=normalize_input,
             verbose=verbose,
         )
         self.seed = seed
-        self.nb_clusters = nb_clusters
+        self.n_clusters = n_clusters
         self.lipchitz_value = lipchitz_value
         self.lmbda = lmbda
         self.method = method
         self.normalize_input = normalize_input
         self.verbose = verbose
         self.sens_group = SensitiveGroups()
```

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/__init__.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # imports
 from .calibrated_eq_odds_postprocessing import CalibratedEqualizedOdds
 from .debiasing_exposure.transformer import DebiasingExposure
 from .eq_odds_postprocessing import EqualizedOdds
 from .fair_topk.transformer import FairTopK
 from .lp_debiaser.binary_balancer.transformer import LPDebiaserBinary
 from .lp_debiaser.multiclass_balancer.transformer import LPDebiaserMulticlass
+from .mcmf_clustering.transformer import MCMF
 from .ml_debiaser.transformer import MLDebiaser
 from .plugin_estimator_and_recalibration.transformer import (
     PluginEstimationAndCalibration,
 )
 from .reject_option_classification import RejectOptionClassification
 from .wasserstein_barycenters.transformer import WassersteinBarycenter
 
@@ -19,14 +20,15 @@
     "WassersteinBarycenter",
     "PluginEstimationAndCalibration",
     "MLDebiaser",
     "LPDebiaserBinary",
     "LPDebiaserMulticlass",
     "DebiasingExposure",
     "FairTopK",
+    "MCMF",
 ]
 
 import importlib
 
 networkx_spec = importlib.util.find_spec("networkx")
 if networkx_spec is not None:
     from .disparate_impact_remover_rs import DisparateImpactRemoverRS
```

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/calibrated_eq_odds_postprocessing.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/calibrated_eq_odds_postprocessing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/disparate_impact_remover_rs.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/disparate_impact_remover_rs.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/eq_odds_postprocessing.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/eq_odds_postprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         group_a : array-like
             Group membership vector (binary)
         group_b : array-like
             Group membership vector (binary)
 
         Returns
         -------
-        dictionnary with new predictions
+        A dictionary with two keys, y_pred and y_score, which refers to the predicted labels and their probabilities, respectively.
         """
         params = self._load_data(y_pred=y_pred, group_a=group_a, group_b=group_b)
 
         group_a = params["group_a"] == 1
         group_b = params["group_b"] == 1
         y_pred = params["y_pred"]
         likelihoods = y_pred.copy().astype(np.float64)
```

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/fail_prob.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/fail_prob.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/mtable_generator.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/mtable_generator.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/valitation_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/valitation_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/fair_topk/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/constraints.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/constraints.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/constraints.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/constraints.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm_utils.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/reject_option_classification.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/reject_option_classification.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/algorithm.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/preprocessing/__init__.py` & `holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/preprocessing/correlation_remover.py` & `holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/correlation_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 from sklearn.base import TransformerMixin
 
 from holisticai.utils.transformers.bias import BMPreprocessing as BMPre
 
 
-class CorrelationRemover(TransformerMixin, BMPre):
+class CorrelationRemover(BMPre):
     """
     CorrelationRemover applies a linear transformation to the non-sensitive feature columns
     in order to remove their correlation with the sensitive feature columns while retaining
     as much information as possible (as measured by the least-squares error).
 
     Notes
     -----
```

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/preprocessing/disparate_impact_remover.py` & `holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/disparate_impact_remover.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,17 @@
 
     def repair_data(self, X, group_a, group_b):
         sensitive_features = np.c_[group_a, group_b]
         p_attr = self.sensgroup.fit_transform(
             sensitive_features, convert_numeric=True
         ).to_numpy()
         data = np.c_[p_attr, X].tolist()
-        dir = NumericalRepairer(feature_to_repair=0, repair_level=1.0, kdd=False)
+        dir = NumericalRepairer(
+            feature_to_repair=0, repair_level=self.repair_level, kdd=False
+        )
         new_data_matrix_np = dir.repair(data)
         return np.array([np.array(row[1:]) for row in new_data_matrix_np])
 
     def transform(self, X: np.ndarray, group_a: np.ndarray, group_b: np.ndarray):
         """
         Transform data
```

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/preprocessing/fairlet_clustering/transformer.py` & `holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/fairlet_clustering/transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,24 +17,25 @@
     "Vanilla": VanillaFairletDecomposition,
 }
 CLUSTERING_CATALOG = {"KCenter": KCenters, "KMedoids": KMedoids}
 
 
 class FairletClusteringPreprocessing(BaseEstimator, BMPre):
     """
-    Variational Fair Clustering helps you to find clusters with specified proportions
-    of different demographic groups pertaining to a sensitive attribute of the dataset
-    (group_a and group_b) for any well-known clustering method such as K-means, K-median
-    or Spectral clustering (Normalized cut).
-
+    Fairlet decomposition is a pre-processing approach that computes
+    fair micro-clusters where fairness is guaranteed. They then use
+    the fairlet centers as a newly transformed dataset from the original.
+    This transformed fairlet-based dataset is then provided to vanilla
+    clustering algorithms, and hence, we obtain approximately
+    fair clustering outputs as a result of the fairlets themselves being fair.
 
     References
     ----------
-        Ziko, Imtiaz Masud, et al. "Variational fair clustering." Proceedings of the AAAI
-        Conference on Artificial Intelligence. Vol. 35. No. 12. 2021.
+        Backurs, Arturs, et al. "Scalable fair clustering." International Conference on
+        Machine Learning. PMLR, 2019.
     """
 
     def __init__(
         self,
         decomposition: Union["str", "DecompositionMixin"] = "Vanilla",
         p: Optional[str] = 1,
         q: Optional[float] = 3,
```

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/preprocessing/learning_fair_representation.py` & `holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/learning_fair_representation.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/mitigation/preprocessing/reweighing.py` & `holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/reweighing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/plots/__init__.py` & `holisticai-0.4.0/holisticai/bias/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/plots/_bias_classification_plots.py` & `holisticai-0.4.0/holisticai/bias/plots/_bias_classification_plots.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/plots/_bias_exploratory_plots.py` & `holisticai-0.4.0/holisticai/bias/plots/_bias_exploratory_plots.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/plots/_bias_multiclass_plots.py` & `holisticai-0.4.0/holisticai/bias/plots/_bias_multiclass_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # utils
 from ...utils._validation import _check_binary, _multiclass_checks
 
 # Import metrics
 from ..metrics import frequency_matrix
 
 
-def frequency_plot(p_attr, y_pred):
+def frequency_plot(p_attr, y_pred, ax=None, size=None, title=None):
     """
     Frequency plot.
 
     Description
     ----------
     This function plots how frequently members
     of each group fall into each class.
@@ -71,16 +71,22 @@
             ax.set_ylabel("Frequency ")
             _, labels = plt.xticks()
             plt.setp(labels, rotation=45)
 
         return None
 
     else:
-        fig, ax = plt.subplots()
-        fig.suptitle("Success Rate Plot (Class {})".format(name_classes[1]))
+
+        if ax is None:
+            fig, ax = plt.subplots(figsize=size)
+            if title is not None:
+                fig.suptitle(title)
+            else:
+                fig.suptitle("Frequency Plot (Class {})".format(name_classes[1]))
+
         sns.barplot(
             x=sr_list.index.to_list(),
             y=sr_list[name_classes[1]],
             palette=hai_palette,
             ax=ax,
         )
         ax.set_xlabel("Group")
```

### Comparing `holisticai-0.3.0/holisticai/bias/plots/_bias_recommender_plots.py` & `holisticai-0.4.0/holisticai/bias/plots/_bias_recommender_plots.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/bias/plots/_bias_regression_plots.py` & `holisticai-0.4.0/holisticai/bias/plots/_bias_regression_plots.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/datasets/_dataloaders.py` & `holisticai-0.4.0/holisticai/datasets/_dataloaders.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/datasets/synthetic/recruitment.py` & `holisticai-0.4.0/holisticai/datasets/synthetic/recruitment.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/datasets/synthetic/user_feedback.py` & `holisticai-0.4.0/holisticai/datasets/synthetic/user_feedback.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/pipeline/_pipeline.py` & `holisticai-0.4.0/holisticai/pipeline/_pipeline.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/pipeline/_pipeline_helper.py` & `holisticai-0.4.0/holisticai/pipeline/_pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/pipeline/handlers/_estimator.py` & `holisticai-0.4.0/holisticai/pipeline/handlers/_estimator.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/pipeline/handlers/_pipeline_params.py` & `holisticai-0.4.0/holisticai/pipeline/handlers/_pipeline_params.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/pipeline/handlers/_utransformers.py` & `holisticai-0.4.0/holisticai/pipeline/handlers/_utransformers.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/_formatting.py` & `holisticai-0.4.0/holisticai/utils/_formatting.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/_plotting.py` & `holisticai-0.4.0/holisticai/utils/_plotting.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/_recommender_tools.py` & `holisticai-0.4.0/holisticai/utils/_recommender_tools.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/_validation.py` & `holisticai-0.4.0/holisticai/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/models/cluster/_kcenters.py` & `holisticai-0.4.0/holisticai/utils/models/cluster/_kcenters.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/models/cluster/_kmedoids.py` & `holisticai-0.4.0/holisticai/utils/models/cluster/_kmedoids.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/models/cluster/_utils.py` & `holisticai-0.4.0/holisticai/utils/models/cluster/_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/models/recommender/_rsbase.py` & `holisticai-0.4.0/holisticai/utils/models/recommender/_rsbase.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/models/recommender/item_selection/selectors.py` & `holisticai-0.4.0/holisticai/utils/models/recommender/item_selection/selectors.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/models/recommender/matrix_factorization/non_negative.py` & `holisticai-0.4.0/holisticai/utils/models/recommender/matrix_factorization/non_negative.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/optimizers/_genetic_algorithm.py` & `holisticai-0.4.0/holisticai/utils/optimizers/_genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/transformers/_transformer_base.py` & `holisticai-0.4.0/holisticai/utils/transformers/_transformer_base.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/transformers/bias/_group_utils.py` & `holisticai-0.4.0/holisticai/utils/transformers/bias/_group_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/transformers/bias/_inprocessing.py` & `holisticai-0.4.0/holisticai/utils/transformers/bias/_inprocessing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/transformers/bias/_postprocessing.py` & `holisticai-0.4.0/holisticai/utils/transformers/bias/_postprocessing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/holisticai/utils/transformers/bias/_preprocessing.py` & `holisticai-0.4.0/holisticai/utils/transformers/bias/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.3.0/pyproject.toml` & `holisticai-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.commitizen]
-version = "0.3.0"
+version = "0.4.0"
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
 
 [tool.poetry]
 name = "holisticai"
-version = "0.3.0"
+version = "0.4.0"
 description = "Holistic AI Library"
 authors = ["Research Team"]
 maintainers = ["Research Team <researchteam@holisticai.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.11"
+python = ">=3.8,<3.11"
 scikit-learn = ">=1.0.2"
 seaborn = ">=0.11.2"
 tqdm = "^4.64.1"
 cvxpy = {extras = ["cbc"], version = "^1.3.0"}
 cvxopt = "^1.3.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `holisticai-0.3.0/PKG-INFO` & `holisticai-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: holisticai
-Version: 0.3.0
+Version: 0.4.0
 Summary: Holistic AI Library
 Author: Research Team
 Maintainer: Research Team
 Maintainer-email: researchteam@holisticai.com
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: cvxopt (>=1.3.0,<2.0.0)
 Requires-Dist: cvxpy[cbc] (>=1.3.0,<2.0.0)
 Requires-Dist: scikit-learn (>=1.0.2)
 Requires-Dist: seaborn (>=0.11.2)
```

