# FeatAug-DETR

This is the official implementation of the paper "[FeatAug-DETR: Enriching One-to-Many Matching for DETRs with Feature Augmentation]". 

Authors: Rongyao Fang, Peng Gao, Aojun Zhou, Yingjie Cai, Si Liu, Jifeng Dai, Hongsheng Li

The codes and model checkpoints will be released very soon!

## Model ZOO

We provide a set of results:

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
<td align="center">24</td>
<td align="center">49.9</td>
</tr>
</tr>
 <tr><td align="left">H-Deformable-DETR + tricks + FeatAug-Flip</a></td>
<td align="center">R50</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">49.4</td>
</tr>
</tr>
 <tr><td align="left">H-Deformable-DETR + tricks + FeatAug-Flip</a></td>
<td align="center">R50</td>
<td align="center">300</td>
<td align="center">24</td>
<td align="center">50.4</td>
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
<td align="center">49.0, 49.6</td>
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
<tr><td align="left">Deformable-DETR + tricks + DataAug</a></td>
<td align="center">Swin Tiny</td>
<td align="center">300</td>
<td align="center">48</td>
<td align="center">53.3</td>
</tr>
</tr>
 <tr><td align="left">Deformable-DETR + tricks + FeatAug-FC</a></td>
<td align="center">Swin Tiny</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">50.9</td>
</tr>
</tr>
 <tr><td align="left">Deformable-DETR + tricks + FeatAug-FC</a></td>
<td align="center">Swin Tiny</td>
<td align="center">300</td>
<td align="center">24</td>
<td align="center">52.7</td>
</tr>
<tr><td align="left">Deformable-DETR</a></td>
<td align="center">Swin Large</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">51.0</td>

<tr><td align="left">Deformable-DETR</a></td>
<td align="center">Swin Large</td>
<td align="center">300</td>
<td align="center">36</td>
<td align="center">53.7</td>
</tr>
</tr>
 <tr><td align="left">Deformable-DETR + tricks</a></td>
<td align="center">Swin Large</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">54.5</td>
</tr>
</tr>
 <tr><td align="left">Deformable-DETR + tricks</a></td>
<td align="center">Swin Large</td>
<td align="center">300</td>
<td align="center">36</td>
<td align="center">56.3</td>
</tr>
</tr>
 <tr><td align="left">Deformable-DETR + tricks + DataAug</a></td>
<td align="center">Swin Large</td>
<td align="center">300</td>
<td align="center">48</td>
<td align="center">57.0</td>
</tr>
</tr>
 <tr><td align="left">Deformable-DETR + tricks + FeatAug-FC</a></td>
<td align="center">Swin Large</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">55.8</td>
</tr>
</tr>
 <tr><td align="left">Deformable-DETR + tricks + FeatAug-FC</a></td>
<td align="center">Swin Large</td>
<td align="center">300</td>
<td align="center">24</td>
<td align="center">57.1</td>
</tr>
 <tr><td align="left">Deformable-DETR + tricks + FeatAug-FC [topk=300]</a></td>
<td align="center">Swin Large</td>
<td align="center">900</td>
<td align="center">24</td>
<td align="center">57.6</td>
</tr>
</tr>
 <tr><td align="left">H-Deformable-DETR + tricks + FeatAug-Flip</a></td>
<td align="center">Swin Large</td>
<td align="center">300</td>
<td align="center">12</td>
<td align="center">56.4</td>
</tr>
</tr>
 <tr><td align="left">H-Deformable-DETR + tricks + FeatAug-Flip</a></td>
<td align="center">Swin Large</td>
<td align="center">300</td>
<td align="center">24</td>
<td align="center">57.6</td>
</tr>
 <tr><td align="left">H-Deformable-DETR + tricks + FeatAug-Flip [topk=300]</a></td>
<td align="center">Swin Large</td>
<td align="center">900</td>
<td align="center">24</td>
<td align="center">58.3</td>
</tr>
</tbody></table>

