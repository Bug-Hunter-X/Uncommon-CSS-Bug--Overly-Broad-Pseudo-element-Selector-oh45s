# Uncommon CSS Bug: Overly Broad Pseudo-element Selector

This repository demonstrates an uncommon CSS bug related to overly broad selectors for pseudo-elements (`:before` and `:after`). The bug occurs when a pseudo-element selector unintentionally affects other elements, potentially leading to unexpected visual or functional behavior.

## Bug Description
The primary issue lies in the selector's specificity.  An overly broad selector applied to a pseudo-element can inadvertently impact elements within the same container that also use pseudo-elements. This is particularly problematic when different pseudo-elements require distinct styles.

## Solution
The solution involves refining the selector to target the specific element where the pseudo-element should be applied. This can involve using more precise class names or leveraging the combinator and parent-child relationships within the CSS structure to avoid unintentional cascading styles.