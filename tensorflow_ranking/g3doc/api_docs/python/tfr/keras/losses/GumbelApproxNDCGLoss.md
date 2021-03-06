<div itemscope itemtype="http://developers.google.com/ReferenceObject">
<meta itemprop="name" content="tfr.keras.losses.GumbelApproxNDCGLoss" />
<meta itemprop="path" content="Stable" />
<meta itemprop="property" content="__call__"/>
<meta itemprop="property" content="__init__"/>
<meta itemprop="property" content="from_config"/>
<meta itemprop="property" content="get_config"/>
</div>

# tfr.keras.losses.GumbelApproxNDCGLoss

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api" align="left">

<td>
  <a target="_blank" href="https://github.com/tensorflow/ranking/tree/master/tensorflow_ranking/python/keras/losses.py">
    <img src="https://www.tensorflow.org/images/GitHub-Mark-32px.png" />
    View source on GitHub
  </a>
</td>
</table>

For Gumbel approximate NDCG loss.

Inherits From: [`ApproxNDCGLoss`](../../../tfr/keras/losses/ApproxNDCGLoss.md)

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>tfr.keras.losses.GumbelApproxNDCGLoss(
    reduction=tf.losses.Reduction.AUTO, name=None, lambda_weight=None,
    sample_size=8, temperature=1.0, seed=None
)
</code></pre>

<!-- Placeholder for "Used in" -->

<!-- Tabular view -->

 <table class="properties responsive orange">
<tr><th colspan="2"><h2 class="add-link">Args</h2></th></tr>

<tr>
<td>
`reduction`
</td>
<td>
(Optional) Type of `tf.keras.losses.Reduction` to apply to
loss. Default value is `AUTO`. `AUTO` indicates that the reduction
option will be determined by the usage context. For almost all cases
this defaults to `SUM_OVER_BATCH_SIZE`. When used with
`tf.distribute.Strategy`, outside of built-in training loops such as
`tf.keras` `compile` and `fit`, using `AUTO` or `SUM_OVER_BATCH_SIZE`
will raise an error. Please see this custom training [tutorial](https://www.tensorflow.org/tutorials/distribute/custom_training)
for more details.
</td>
</tr><tr>
<td>
`name`
</td>
<td>
Optional name for the op.
</td>
</tr>
</table>

## Methods

<h3 id="from_config"><code>from_config</code></h3>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>@classmethod</code>
<code>from_config(
    config
)
</code></pre>

Instantiates a `Loss` from its config (output of `get_config()`).

<!-- Tabular view -->

 <table class="properties responsive orange">
<tr><th colspan="2">Args</th></tr>

<tr>
<td>
`config`
</td>
<td>
Output of `get_config()`.
</td>
</tr>
</table>

<!-- Tabular view -->

 <table class="properties responsive orange">
<tr><th colspan="2">Returns</th></tr>
<tr class="alt">
<td colspan="3">
A `Loss` instance.
</td>
</tr>

</table>

<h3 id="get_config"><code>get_config</code></h3>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>get_config()
</code></pre>

Returns the config dictionary for a `Loss` instance.

<h3 id="__call__"><code>__call__</code></h3>

<a target="_blank" href="https://github.com/tensorflow/ranking/tree/master/tensorflow_ranking/python/keras/losses.py">View
source</a>

<pre class="devsite-click-to-copy prettyprint lang-py tfo-signature-link">
<code>__call__(
    y_true, y_pred, sample_weight=None
)
</code></pre>

See _RankingLoss.
