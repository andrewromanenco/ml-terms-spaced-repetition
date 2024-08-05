#language, #generativeAI

A [[parameter-efficient tuning|parameter efficient tuning]] mechanism
that learns a &quot;prefix&quot; that the system prepends to the
actual [[prompt|prompt]].

One variation of prompt tuning—sometimes called <strong>prefix tuning</strong>—is to
prepend the prefix at <em>every layer</em>. In contrast, most prompt tuning only
adds a prefix to the [[input layer|input layer]].

<section class="expandable">

<h4 class="showalways" id="click-the-icon-to-learn-more-about-prefixes." data-text=" Click the icon to learn more about prefixes. " tabindex="-1">
Click the icon to learn more about prefixes.
</h4>

<div class="expand-background">
For prompt tuning, the "prefix" (also known as a "soft prompt") is a
handful of learned, task-specific vectors prepended to the text token
embeddings from the actual prompt. The system learns the soft prompt by
freezing all other model parameters and fine-tuning on a specific task.
</div>

<hr />
</section>

