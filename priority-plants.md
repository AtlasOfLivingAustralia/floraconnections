---
layout: onecolumn

title: "Priority Plants Finder"
---

After the catastrophic 2019-20 bushfires, the Australian Government [published a list of over 450 plant species](https://www.awe.gov.au/environment/biodiversity/bushfire-recovery/bushfire-impacts/priority-plants) that were of the highest priority for urgent management intervention to support their recovery. Some of the species on this list were threatened to begin with, but many species had so much of their range burned that they may not be able to recover by themselves. This list also includes plants that are currently [under assessment for recognition as threatened species under the EPBC Act](https://www.environment.gov.au/sprat-public/action/fpal-submit) as of March 2022.

The priority list that we have below omits species that are already listed as threatened or endanged -- instead, we are calling attention to priority plants that still need to be assessed for Threatened status. Information on any of these plants may help secure funding for their future management and conservation. 

At this time, none of our target species are endemic to the Northern Territory.

<div class="controls">
    <p>
    <strong>Show species endemic to...</strong>
    </p><p>
    <button type="button" class="control" data-filter="all">Australia</button>
    <button type="button" class="control" data-filter=".nsw">NSW/ACT</button>
    <button type="button" class="control" data-filter=".vic">VIC</button>
    <button type="button" class="control" data-filter=".wa">WA</button>
    <button type="button" class="control" data-filter=".tas">TAS</button>
    <button type="button" class="control" data-filter=".sa">SA</button>
    <button type="button" class="control" data-filter=".qld">QLD</button>
    </p>
</div>

<div class="container">

    {% include card_code.html %}

    <div class="gap"></div>
    <div class="gap"></div>
    <div class="gap"></div>
    <div class="gap"></div>
</div>

<script src="_assets/js/mixitup.min.js"></script>

<script>
    var containerEl = document.querySelector('.container');

    var mixer = mixitup(containerEl, {
        load: {
            filter: 'all',
            sort: 'order:asc'
        },
        
        controls: {
            toggleLogic: 'or'
        }
    });
</script>
