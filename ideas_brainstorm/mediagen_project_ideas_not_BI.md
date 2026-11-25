# Ideas out of data and BI-related fields

## Bedazzling and craft DIY. Exploding Topics reports 301,000 monthly searches and 2,733% growth over the past two years. 
Image generation for designs, tutorial clips, and narrated steps all fit. You already teach step-by-step sewing to beginners, so you would know what a good tutorial looks like, and that matters for human evaluation. Strong. 
https://explodingtopics.com/media-exploding-topics

## Winter 2026–27 weather predictions. Searches are high, with 50K+ searches in one trend feed. 
Pull real forecast data, render deterministic charts in code, narrate a briefing with Kokoro, and add a short video. 
This fits the data-grounding rule well and stays relevant through the deadline.

## Interview simulation. The weak point is evaluation. Scoring an answer's quality needs human labels, because an LLM judge isn't deterministic. T
he Whisper round-trip can check the speech, but not whether the feedback is good. There is also a misuse concern: realistic synthetic recruiters could be used for deception, so the product would need to be clearly framed as practice.

## Personal gift books. The rubric fits well. Deterministic checks can verify that names, dates, and captions match the input data exactly. 
The catch is privacy. If the book uses personal photos, you're processing real people's likenesses, so the design should use the user's own photos only with consent, or an illustration style that avoids identifiable faces. The cost is high but measurable, and per-page cost reporting shows that directly.

## Style guide by figure. This is the strongest option. Palette contrast, size charts, and measurement conversions can all be computed and verified in code, and the image model only generates the visuals. For the 100-record dataset, use synthetic figures rather than real body data, which avoids storing personal measurements. 
Your sewing background would also make human evaluation of fit and style credible, which is a genuine advantage.

## Here are four additional ideas that fit the rubric well. For each, the deterministic check is what I'd use to verify quality.

1. Data-grounded explainer videos from open data
Take a public dataset (city transit, air quality, energy prices) and turn it into short narrated videos. Charts are rendered in code from the data, Kokoro narrates a script generated from those same numbers, and Wan 2.2 produces the background footage.

Deterministic check: Whisper transcribes the narration, and every number in it must match the source data.
Batch: 10 video records is enough, which keeps video cost manageable.
Caveat: Video is the expensive part, so the cost-per-asset report will show it clearly.

2. Weekly audio briefings for small-business KPIs
A small business uploads a CSV export of sales or traffic, and the system produces a short narrated weekly briefing in one or more languages, with a rendered chart.

Models: Kokoro for narration, plus an image model for the summary card.
Deterministic check: Numbers in the transcript must match the CSV, and charts come from code, not a model.
Eval: Human ratings on a sample of briefings for clarity and usefulness.
Fit: This matches your SMB advisory experience and your data skills directly.

3. Decodable reading stories for early readers
Short illustrated stories that use only words from an allowed phonics list, with narration for listening practice.

Deterministic check: Every word in the story must come from the allowed list. This is a strict, automatic lexical check, which makes the evaluation unusually clean.
Models: FLUX for illustrations and Kokoro for narration. Whisper can verify the narration matches the text.
Batch: 100 stories is easy to generate.
Caveat: Children's content needs strict filtering, and a teacher or parent should label a sample for readability.

4. Platform-specific product images with code-rendered text
From one product spec sheet (name, size, price, materials), generate images in each platform's aspect ratio. The product photo comes from the image model, but all text overlays (price, size, dimensions) are drawn in code.

Deterministic check: OCR on the final image must match the spec sheet exactly. This directly addresses the "no generated facts" rule, since the image model never writes numbers.
Models: Sana or FLUX for product scenes, plus a second model for short video if you want it.
Fit: This is a narrower, more defensible version of the Etsy idea, focused on generation rather than scheduling.

