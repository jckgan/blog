---
title: "Introducing Nevuqe"
date: 2023-11-28T00:00:00-11:00
updated: 2023-11-28T15:30:00-11:00
tags: ["nevuqe", "ethics", "artificial intelligence", "personal"]
excerpt: "Introducing Nevuqe, a business and brand built from the ground up. Nevuqe is a research organization with the goal of revolutionizing how we interface with the technology that we use on a daily basis. Its aim is to advance towards the seamless incorporation of AGI into our daily lives once it is created."
layout: single
type: post
draft: false
latex: true
---

Introducing Nevuqe, a business and brand built from the ground up. Nevuqe is a research organization with the goal of revolutionizing how we interface with the technology that we use on a daily basis. Its aim is to advance towards the seamless incorporation of AGI into our daily lives once created.

## On AGI: An overview of both benefits & risk-avoidance.

An artificial intelligence singularity event is inevitable; whether it occurs from within the next year or the next thirty years is only extraneous. Our world governments (alongside the citizens & corporations that inhabit them) are collectively presented with an opportunity - one that could significantly enhance the quality of life for billions globally, effectively eliminating and lifting those out of poverty/starvation - humanity could resume the advancement of scientific knowledge - regarding our natural world - at an unprecedented speed; we could rectify existing flaws in our sociopolitical economic structures, and we could potentially begin to ameliorate corruptions in our current governmental systems.

However, these scenarios are only hypotheticals; the practicality regarding the implementation of AGI into our societal systems will be seen as yet to be observed. It's a logical assumption that our vision of the future can be corrupted; it can be predicated upon not only by pessimistic or overly optimistic viewpoints, but also the desire for our lives to remain as they are. We can currently only attempt to construct logical, unbiased assumptions concerning what our societies will succumb to/function as, but we can only be certain once AGI has been achieved. Whether the product of AGI is positive or negative is ultimately a topic that international societies need to brace for, and rapidly acclimatise to. With the eventual enabling of open discourse regarding AGI, it's for humanities common interest that all parties involved in this discussion are aware of these few certainties:

Firstly, we're placed with a collaborative requirement to ensure that AGI isn't treated merely as a consumer commodity; AGI, fundamentally, should not be seen as a product to be bought and sold. This is a substantial addition to humanity, its nature being juxtaposed between an arsenal and a tool for collective good. The release of AGI into our world should not be top-down; the access and control of AGI should be democratised amongst the working class, creatives, and public intellects. An open discourse regarding the implementation, replacement, and function of AGI in our societal structures is necessary - but the means by which we achieve this fair discourse is yet to be decided.

Secondly, it's an inevitability that a consortium of people would aim to systematically utilise all available resources and capabilities in their leverage in order to effectively govern every aspect of AGI for their own self-interest; their motivations may range from financial and hierarchical gains - to the sheer desire for societal disruption. Hence, this is again my reiteration for the aforementioned imminent democratisation of access/influence to AGI once created; if everybody controls and influences the direction of AGI, then this becomes a non-issue (to some extent). These people will guise themselves under a (faux) compassion for humanity - they will assert the fact that they want a more equitable implementation of AGI into society - but will simultaneously enact regulations for their self-interests; as seen in history, we cannot be entirely correct in appointing somebody to lead with clear intentions, so hence democratisation and open-discussions are necessary.


> **1914 translation by H. Rackham**
> 
> But I must explain to you how all this mistaken idea of denouncing pleasure and praising pain was born and I will give you a complete account of the system, and expound the actual teachings of the great explorer of the truth, the master-builder of human happiness. No one rejects, dislikes, or avoids pleasure itself, because it is pleasure, but because those who do not know how to pursue pleasure rationally encounter consequences that are extremely painful. Nor again is there anyone who loves or pursues or desires to obtain pain of itself, because it is pain, but because occasionally circumstances occur in which toil and pain can procure him some great pleasure. To take a trivial example, which of us ever undertakes laborious physical exercise, except to obtain some advantage from it? But who has any right to find fault with a man who chooses to enjoy a pleasure that has no annoying consequences, or one who avoids a pain that produces no resultant pleasure?


{{<figure src="/images/posts/Meta/lorem-ipsum/Pompejanischer_Maler_um.webp" alt="Pompejanischer Maler um 10/20" em="*[Pompejanischer Maler um 10/20](https://commons.wikimedia.org/wiki/File:Pompejanischer_Maler_um_10_20_001.jpg), Public domain, via Wikimedia Commons*">}}


## LaTeX support

You can embed equations inline
{{<latex-inline>}}
\frac{2}{c} e ^{-\frac{c^2}{2}}
{{</latex-inline>}}
or in blocks

{{<latex>}}
|x|_0 = \lim_{p \to 0^{+}} \Bigg(\sum_{i=1}^{n} |x_i|^p\Bigg)^{\frac{1}{p}} = |\{i \mid x_i \neq 0\}| = support(\textbf{x})
{{</latex>}}


## Code highlighting

```c
// datalen = number of bits
void blake256_update(state *S, const uint8_t *data, uint64_t datalen) {
    int left = S->buflen >> 3;
    int fill = 64 - left;

    if (left && (((datalen >> 3)) >= (unsigned) fill)) {
        memcpy((void *) (S->buf + left), (void *) data, fill);
        S->t[0] += 512;
        if (S->t[0] == 0) S->t[1]++;
        blake256_compress(S, S->buf);
        data += fill;
        datalen -= (fill << 3);
        left = 0;
    }

    while (datalen >= 512) {
        S->t[0] += 512;
        if (S->t[0] == 0) S->t[1]++;
        blake256_compress(S, data);
        data += 64;
        datalen -= 512;
    }

    if (datalen > 0) {
        memcpy((void *) (S->buf + left), (void *) data, datalen >> 3);
        S->buflen = (left << 3) + datalen;
    } else {
        S->buflen = 0;
    }
}

// datalen = number of bits
void blake224_update(state *S, const uint8_t *data, uint64_t datalen) {
    blake256_update(S, data, datalen);
}
```
*[Source](https://github.com/monero-project/monero/blob/master/src/crypto/blake256.c), [license](https://github.com/monero-project/monero/blob/master/LICENSE)*


## Other markdown stuff

*Italics*, **Bold**, ***Bold Italics***

1. Lists look like this
2. Second element
3. Third element
    - First sub element
    - Second sub element[^1]

[^1]: This is the first footnote.


|Tables|look|like this|
|------|----|---------|
|Sed ut perspiciatis|unde omnis iste natus error sit|voluptatem accusantium|
|doloremque laudantium,| totam rem aperiam|, eaque ipsa quae ab illo|
|inventore veritatis et| quasi architecto beatae|vitae dicta sunt explicabo.|
|{{<latex-inline>}}\forall x \; \|f(x)\| \geq 17{{</latex-inline>}}|LaTeX works everywhere|:)|


```goat
      .               .                .               .--- 1          .-- 1     / 1
     / \              |                |           .---+            .-+         +
    /   \         .---+---.         .--+--.        |   '--- 2      |   '-- 2   / \ 2
   +     +        |       |        |       |    ---+            ---+          +
  / \   / \     .-+-.   .-+-.     .+.     .+.      |   .--- 3      |   .-- 3   \ / 3
 /   \ /   \    |   |   |   |    |   |   |   |     '---+            '-+         +
 1   2 3   4    1   2   3   4    1   2   3   4         '--- 4          '-- 4     \ 4

```