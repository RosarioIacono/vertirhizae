+++
date = '2025-10-24T08:16:09+02:00'
draft = false
title = 'Measuring the Unseen: How Simple Leaf Shapes Reveal the Impact of Mycorrhizae in Vertical Farming'
+++

In the Vertirhizae project, we are exploring a powerful synergy: enhancing tomato growth in the high-tech environment of vertical farming through a natural partnership with mycorrhizal fungi. To understand this hidden relationship, we've turned to a precise and powerful tool: digital image analysis. While the world of plant phenotyping is vast, our focus is razor-sharp: we use the open-source software Fiji (ImageJ) to measure fundamental leaf traits that serve as a window into plant vitality.

<!--more-->

### **Why Leaf Area and Perimeter?**

In the controlled, often soil-less context of vertical farming, a plant's resources are meticulously managed. When we introduce mycorrhizal fungi, we expect a shift in how efficiently the plant uses these resources. We need a simple, non-destructive, and highly accurate way to measure the outcome of this shift.

This is where the basic geometry of a leaf becomes incredibly informative.

*   **Total Leaf Area:** This is a direct measure of the plant's photosynthetic factory. A larger leaf area typically means a greater capacity to capture light and produce energy for growth and fruit development. By tracking leaf area over time, we can see if tomatoes colonized by mycorrhizae are building their photosynthetic machinery more effectively.

*   **Leaf Perimeter:** The perimeter measures the outer boundary of the leaf. On its own, it's a simple metric. But when combined with area, it reveals much more.

### **The Key Metric: The Shape Compactness Index (P²/A)**

Our analysis goes beyond just measuring two independent numbers. The true power of our method lies in a specific calculation: the Shape Compactness Index, expressed as the ratio P²/A (the square of the Perimeter divided by the Area).

This index is a powerful dimensionless descriptor of leaf shape complexity.

Imagine two leaves with the exact same area. One is a perfect, compact circle, while the other is a sprawling, deeply lobed tomato leaf. The compact circular leaf will have a much smaller perimeter for the same area, resulting in a lower P²/A value (close to 12.6). The lobed tomato leaf, with its extensive, indented edges, will have a much larger perimeter, yielding a higher P²/A value.

For our tomatoes, this isn't about aesthetics; it's about development. A shift in the Compactness Index can indicate changes in leaf morphology influenced by the plant's physiological state. A change in this value (either more or less complex) could suggest different developmental patterns, potentially influenced by the improved nutrient and water uptake provided by the mycorrhizal fungi.

**Our Workflow: From Leaf to Data with Fiji**

Our process is streamlined for accuracy and reproducibility:

1.  **Image Acquisition:** We photograph tomato leaves against a high-contrast background at regular intervals throughout their growth cycle. Consistency in lighting and camera setup is key, as highlighted by researchers like Martin et al. (2020), to ensure every measurement is comparable.
2.  **Thresholding in Fiji:** We import the images into Fiji and use its thresholding tools. This process cleanly separates the leaf (the region of interest) from the background, converting the image into a binary black-and-white silhouette.
3.  **Automated Measurement:** With a single click, Fiji’s analysis tools measure the **Area (A)** and **Perimeter (P)** of this silhouette with pixel-level precision. We then export this raw data.
4.  **Calculating the Area Index:** In our data analysis software, we automatically calculate the **A/P²** ratio for every single leaf. This creates a robust dataset of morphological traits for every plant in our study—both the mycorrhized group and the control group.

**Connecting the Dots to Mycorrhizae**

So, how does measuring shape tell us about an invisible fungal partnership?

The connection is indirect but powerful. We know from established science that mycorrhizae act as an extension of the root system, enhancing the plant's uptake of phosphorus, water, and other nutrients. This "bio-fertilization" reduces plant stress and allows for more optimal growth.

In Vertirhizae, we hypothesize that this improved resource status will be reflected in the leaves' development. By statistically comparing the **Area, Perimeter, and Area Index (A/P²)** between our treated and control groups, we can determine if mycorrhization leads to:

By statistically comparing the Area, Perimeter, and Shape Compactness Index (P²/A) between our treated and control groups, we can determine if mycorrhization leads to:

* Larger leaves (increased Area), indicating greater vigor.
* A measurable change in leaf shape complexity (a shift in the P²/A Index), suggesting a morphological adaptation to the improved nutritional environment.

This quantitative approach allows us to move from a qualitative observation ("the mycorrhized plants look better") to a data-driven conclusion ("the mycorrhized plants show a statistically significant 15% increase in leaf area and a distinct shift in leaf shape compactness by week 6").

By focusing on these fundamental geometric traits with Fiji, the Vertirhizae project is building a clear, reproducible link between a natural biological alliance and the measurable architecture of plant growth in the vertical farms of the future.