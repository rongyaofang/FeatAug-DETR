# FeatAug-DETR

This is the official implementation of the paper "[FeatAug-DETR: Enriching One-to-Many Matching for DETRs with Feature Augmentation]". 

Authors: Rongyao Fang, Peng Gao, Aojun Zhou, Yingjie Cai, Si Liu, Jifeng Dai, Hongsheng Li

The codes and model checkpoints will be released very soon!

## Model ZOO

We provide a set of baseline results and trained models available for download:

### Models with the ResNet-50 backbone
<table><tbody>
<!-- START TABLE -->
<!-- TABLE HEADER -->
<th valign="bottom">Name</th>
<th valign="bottom">Backbone</th>
<th valign="bottom">query</th>
<th valign="bottom">epochs</th>
<th valign="bottom">AP</th>
<!-- TABLE BODY -->
 <tr><td align="left">Deformable-DETR</a></td>
<td align="center">R50</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">43.7</td>
 <tr><td align="left">Deformable-DETR</a></td>
<td align="center">R50</td>
<td align="center">300</td>
<td align="center">36</td>
<td align="center">46.8</td>
</tr>
</tr>
 <tr><td align="left">Deformable-DETR + tricks</a></td>
<td align="center">R50</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">47.0</td>
</tr>
</tr>
 <tr><td align="left">Deformable-DETR + tricks</a></td>
<td align="center">R50</td>
<td align="center">300</td>
<td align="center">36</td>
<td align="center">49.0</td>
</tr>
</tr>
 <tr><td align="left">Deformable-DETR + tricks + DataAug</a></td>
<td align="center">R50</td>
<td align="center">300</td>
<td align="center">48</td>
<td align="center">50.0</td>
</tr>
</tr>
 <tr><td align="left">Deformable-DETR + tricks + FeatAug-FC</a></td>
<td align="center">R50</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">48.7</td>
</tr>
</tr>
 <tr><td align="left">Deformable-DETR + tricks + FeatAug-FC</a></td>
<td align="center">R50</td>
<td align="center">300</td>
<td align="center">36</td>
<td align="center">49.9</td>
</tr>
</tbody></table>

### Models with Swin Transformer backbones

<table><tbody>
<!-- START TABLE -->
<!-- TABLE HEADER -->
<th valign="bottom">Name</th>
<th valign="bottom">Backbone</th>
<th valign="bottom">query</th>
<th valign="bottom">epochs</th>
<th valign="bottom">AP</th>
<!-- TABLE BODY -->
<tr><td align="left">Deformable-DETR</a></td>
<td align="center">Swin Tiny</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">45.3, 46.0</td>
 <tr><td align="left">Deformable-DETR</a></td>
<td align="center">Swin Tiny</td>
<td align="center">300</td>
<td align="center">36</td>
<td align="center">49.0,49.6</td>
</tr>
</tr>
 <tr><td align="left">Deformable-DETR + tricks</a></td>
<td align="center">Swin Tiny</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">49.3</td>
</tr>
</tr>
 <tr><td align="left">Deformable-DETR + tricks</a></td>
<td align="center">Swin Tiny</td>
<td align="center">300</td>
<td align="center">36</td>
<td align="center">51.8</td>
</tr>
</tr>
<tr><td align="left"><a href="configs/two_stage/deformable-detr-hybrid-branch/12eps/swin/swin_tiny_hybrid_branch_lambda1_group6_t1500_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage.sh">H-Deformable-DETR + tricks</a></td>
<td align="center">Swin Tiny</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">50.6</td>
</tr>
</tr>
 <tr><td align="left"><a href="configs/two_stage/deformable-detr-hybrid-branch/36eps/swin/swin_tiny_hybrid_branch_lambda1_group6_t1500_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage.sh">H-Deformable-DETR + tricks</a></td>
<td align="center">Swin Tiny</td>
<td align="center">300</td>
<td align="center">36</td>
<td align="center">53.2</td>
</tr>
<tr><td align="left"><a href="configs/two_stage/deformable-detr-baseline/12eps/swin/swin_large_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage.sh">Deformable-DETR</a></td>
<td align="center">Swin Large</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">51.0</td>

<tr><td align="left"><a href="configs/two_stage/deformable-detr-baseline/36eps/swin/drop_path0.5_swin_large_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage.sh">Deformable-DETR</a></td>
<td align="center">Swin Large</td>
<td align="center">300</td>
<td align="center">36</td>
<td align="center">53.7</td>
</tr>
</tr>
 <tr><td align="left"><a href="configs/two_stage/deformable-detr-baseline/12eps/swin/swin_large_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage.sh">Deformable-DETR + tricks</a></td>
<td align="center">Swin Large</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">54.5</td>
</tr>
</tr>
 <tr><td align="left"><a href="configs/two_stage/deformable-detr-baseline/36eps/swin/drop_path0.5_swin_large_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage.sh">Deformable-DETR + tricks</a></td>
<td align="center">Swin Large</td>
<td align="center">300</td>
<td align="center">36</td>
<td align="center">56.3</td>
</tr>
</tr>
 <tr><td align="left"><a href="configs/two_stage/deformable-detr-hybrid-branch/12eps/swin/swin_large_hybrid_branch_lambda1_group6_t1500_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage.sh">H-Deformable-DETR + tricks</a></td>
<td align="center">Swin Large</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">55.9</td>
</tr>
</tr>
 <tr><td align="left"><a href="configs/two_stage/deformable-detr-hybrid-branch/36eps/swin/drop_path0.5_swin_large_hybrid_branch_lambda1_group6_t1500_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage.sh">H-Deformable-DETR + tricks</a></td>
<td align="center">Swin Large</td>
<td align="center">300</td>
<td align="center">36</td>
<td align="center">57.1</td>
</tr>
</tr>
 <tr><td align="left"><a href="configs/two_stage/deformable-detr-hybrid-branch/12eps/swin/swin_large_hybrid_branch_lambda1_group6_t1500_n900_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage.sh">H-Deformable-DETR + tricks</a></td>
<td align="center">Swin Large</td>
<td align="center">900</td>
<td align="center">12</td>
<td align="center">56.1</td>
</tr>
</tr>
 <tr><td align="left"><a href="configs/two_stage/deformable-detr-hybrid-branch/36eps/swin/drop_path0.5_swin_large_hybrid_branch_lambda1_group6_t1500_n900_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage.sh">H-Deformable-DETR + tricks</a></td>
<td align="center">Swin Large</td>
<td align="center">900</td>
<td align="center">36</td>
<td align="center">57.4</td>
</tr>
 <tr><td align="left"><a href="configs/two_stage/deformable-detr-hybrid-branch/36eps/swin/drop_path0.5_swin_large_hybrid_branch_lambda1_group6_t1500_n900_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage.sh">H-Deformable-DETR + tricks [topk=300]</a></td>
<td align="center">Swin Large</td>
<td align="center">900</td>
<td align="center">36</td>
<td align="center">57.6</td>
</tr>
</tbody></table>

### Improving H-Deformable-DETR with weight decay 0.05

<table><tbody>
<!-- START TABLE -->
<!-- TABLE HEADER -->
<th valign="bottom">Name</th>
<th valign="bottom">Backbone</th>
<th valign="bottom">query</th>
<th valign="bottom">epochs</th>
<th valign="bottom">AP (weight-decay=0.0001)</th>
<th valign="bottom">AP (weight-decay=0.05</th>
<th valign="bottom">download</th>
<!-- TABLE BODY -->
<tr><td align="left"><a href="configs/two_stage/deformable-detr-hybrid-branch/12eps/swin/decay0.05_swin_tiny_hybrid_branch_lambda1_group6_t1500_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage.sh">H-Deformable-DETR + tricks</a></td>
<td align="center">Swin Tiny</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">50.6</td>
<td align="center">51.2</td>
<td align="center"><a href="https://github.com/HDETR/H-Deformable-DETR/releases/download/v0.1/decay0.05_swin_tiny_hybrid_branch_lambda1_group6_t1500_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage_12eps.pth">model</a></td>
</tr>
</tr>
 <tr><td align="left"><a href="configs/two_stage/deformable-detr-hybrid-branch/36eps/swin/decay0.05_swin_tiny_hybrid_branch_lambda1_group6_t1500_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage.sh">H-Deformable-DETR + tricks</a></td>
<td align="center">Swin Tiny</td>
<td align="center">300</td>
<td align="center">36</td>
<td align="center">53.2</td>
<td align="center">53.7</td>
<td align="center"><a href="https://github.com/HDETR/H-Deformable-DETR/releases/download/v0.1/decay0.05_swin_tiny_hybrid_branch_lambda1_group6_t1500_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage_36eps.pth">model</a></td>
</tr>
</tr>
 <tr><td align="left"><a href="configs/two_stage/deformable-detr-hybrid-branch/36eps/swin/decay0.05_drop_path0.5_swin_large_hybrid_branch_lambda1_group6_t1500_n900_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage.sh">H-Deformable-DETR + tricks</a></td>
<td align="center">Swin Large</td>
<td align="center">900</td>
<td align="center">36</td>
<td align="center">57.4</td>
<td align="center">57.8</td>
<td align="center"><a href="https://github.com/HDETR/H-Deformable-DETR/releases/download/v0.1/decay0.05_drop_path0.5_swin_large_hybrid_branch_lambda1_group6_t1500_n900_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage_36eps.pth">model</a></td>
</tr>
 <tr><td align="left"><a href="configs/two_stage/deformable-detr-hybrid-branch/36eps/swin/decay0.05_drop_path0.5_swin_large_hybrid_branch_lambda1_group6_t1500_n900_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage.sh">H-Deformable-DETR + tricks [topk=300]</a></td>
<td align="center">Swin Large</td>
<td align="center">900</td>
<td align="center">36</td>
<td align="center">57.6</td>
<td align="center">57.9</td>
<td align="center"><a href="https://github.com/HDETR/H-Deformable-DETR/releases/download/v0.1/decay0.05_drop_path0.5_swin_large_hybrid_branch_lambda1_group6_t1500_n900_dp0_mqs_lft_deformable_detr_plus_iterative_bbox_refinement_plus_plus_two_stage_36eps.pth">model</a></td>
</tr>
 <tr><td align="left"><a href="">H-Deformable-DETR<sup>deep-encoder</sup> + tricks [topk=300]</a></td>
<td align="center">Swin Large</td>
<td align="center">900</td>
<td align="center">36</td>
<td align="center">NA</td>
<td align="center">58.2</td>
<td align="center"><a href="h">model</a></td>
</tr>
</tbody></table>