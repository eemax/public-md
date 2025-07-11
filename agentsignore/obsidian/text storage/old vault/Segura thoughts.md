We actually should not collect data on PO level initially. We must collect data the whole of:
- whole raw materials that nwg buys.

Wait, wholly map all our factories down to raw materials, what’s their impact on all our materials, or their annual impact and our percentage of their output. We need this in segura. It’s not PO it is **raw material per batch produced** even if we don’t use the whole batch.

So it has so be all raw materials we touch.
Secondly, it can be all materials we touched that year, including the subprocesses.

Only later will we tie them to our PO orders and products as a last step, because we need that deeper data.

So segura is:
- all raw materials batches we touch
- All materials batches incl. subprocesses we touch
- We may want all subprocesses we touch separately as they may combine several material batches. (all processing of the material up until ready for assembly)
- aggregate to PO

On the batches: we need our piece of the batch exactly with impact. If we cannot have it we need the whole batch, their annual output and we have to estimate impact.

In Centric the material library with attributes. Segura we only need the code and impact and link to a raw material batch.

Then we also need cut/sew/assembly on style.   it’s quite easy to estimate by just looking at the factory output. 


Plan:
Even if we don’t collect all now, we certainly need the full structure set up now.
A potential fallback set up in place if we only can report on materials and have no clue on the impacts. We can use an average of production in the same region etc.


Need to get more tightly involved in buying and sourcing also. There is where a lot of collection will happen.