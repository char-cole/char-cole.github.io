---
layout: default
title: insect catalogue
categories: photography insecta
---

# Insecta

Insects are familiar to most people, but not necessarily well understood.
Insects are arthropods (meaning "jointed-foot"), animals which have jointed legs and a segmented body
with an exoskeleton. This includes insects, as well as spiders, crabs,
centipedes, and more.

Insects are most easily distinguished by having 6 legs, which is not true of any other animals except a handful of other closely related arthropods. Centipedes are therefore not insects, nor are snails (they are not even arthropods, but gastropods).

Insects are incredibly diverse and prolific. They are so diverse than by species count, insects alone represent more than half of all known organisms (not just animals!). In addition, despite their small size, insects represent a significant portion of the biomass of Earth - it is thought that there are more ants than humans _by weight_.

Because of the great number of insect species, the extreme difficulty of identifying species confidently, and the lack of comprehensive resources available to laypersons, I make no attempt at truly cataloguing the insects of my area. I simply enjoy the ones around me and celebrate the ones I really like.

Insects are largely divided into families which can generally be distinguished simply by their body shape. These families are often named after the wing structure ("ptera" in the family names means "wing"). Sometimes, the details of the wing structure are not easily seen, but general body shape can usually inform a family-level identification.

Some of the larger families include:
- **coleoptera**, meaning "covered wings", the beetles. Typically, it is quite easy to identify a beetle: unless it is in flight, you won't see its wings. Instead you will see its elytra, the movable armor plates which cover its wings. Beetles tend to have a "fully armored" look.
- **diptera**, meaning "two-winged", the true flies. If you can definitely identify a specimen as having only two wings, it is probably a diptera. Often the wings are folded back on the body at an angle (picture a housefly).
- **hymenoptera**, meaning "clasped wings". These are ants, bees, and wasps (but not termites!). Their name comes from a small hook which latches their front and back wings together - this can't be seen without careful examination, but most people are familiar with the body shape of bees, wasps, and ants. The hardest part of hymenoptera identification is the large number of diptera which mimic the shape and coloration of bees: without being familiar with all the local bee species, an observer should count the number of wings to be sure which family they are looking at. Hymenoptera can often sting; diptera cannot.

{% for page in site.insecta %}
<a href="{{page.url}}">{{ page.heading }}</a>
{% endfor %}
