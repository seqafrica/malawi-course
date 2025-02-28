# Mysterious Asgard Archaea?

Shortly after this was published:
<https://www.science.org/content/article/strange-tentacled-microbe-may-resemble-ancestor-complex-life>

... detailing the possible missing link between Archaea and Eukariota
... three apparent Asgard Archaea showed up in a run!

The Asgard Archaea have more genes in common with eukariotes than other
archaea and exhibit structural features (tentacles, bubbles) like them.

When three samples showed up in a bacterial run that matched nothing
known, I checked them against the GTDB-TK: <https://gtdb.ecogenomic.org/>.

GTDB is a highly accurate typology, based on ANI on a conserved set of 120(?)
proteins, of 107,000 bacteria and 12,000 archaea species.

Bingo?!

```email
Fra: Marco van Zwetselaar <zwets@zwets.com>
Sendt: 22. december 2022 15:35:48
Til: Frank Møller Aarestrup; Philip Thomas Lanken Conradsen Clausen
Emne: Asgard microbes
 
Did you read this?

    https://www.science.org/content/article/strange-tentacled-microbe-may-resemble-ancestor-complex-life

Just hád to check my recent GTDB run, as I remember ditching 9 Archaea from my 2900 assemblies. Yes, we have 5 Asgards:

Dodoma FFDD_878-5873215 d__Archaea;p__Asgardarchaeota;c__Heimdallarchaeia RED 0.4622
Tabora FFTB_11368 d__Archaea;p__Asgardarchaeota;c__Wukongarchaeia RED 0.3897
Tabora FFTB_33862 d__Archaea;p__Asgardarchaeota;c__Heimdallarchaeia RED 0.4606
# omitted 2, both Tabora; one mixed Archaea, one contaminated with bacteria

The RED is relative evolutionary distance from the rank to which they could be classified. Clearly they don't match anything in Archaeal RefSeq, with assignment failing to anything below class rank.

The weird thing however is that these isolates (from culture) have plenty of reads, no apparent human or vector contamination, no bacteria mix-in, but they spectacularly fail to assemble. Not just to 3500 contigs, but to 15,000 or more contigs.

Any idea what is going on here??
```

What was notable is that the genomes didn't assemble well at all, and their
RED from the the class rank to which they were assigned (Wukong/Heimdallarchea).

Response from prof Frank in Copenhagen:

```email
On 22/12/2022 17:39, Frank Møller Aarestrup wrote:

Are they still available as frozen stocks?

It could be contaminations of the broth or growth plates. But should ASAP be investigated.

Perhaps I should fly down?

F
```

What did I discover?

The assemblies are here:

 * [FFDD_878-5873215.fna.gz](https://zwets.it/bix2/mystery/FFDD_878-5873215.fna.gz)
 * [FFTB_11368.fna.gz](https://zwets.it/bix2/mystery/FFTB_11368.fna.gz)
 * [FFTB_33862.fna.gz](https://zwets.it/bix2/mystery/FFTB_33862.fna.gz)

You find out, and explain:

 - What were these isolates?
 - What was my mistake, why did I find what I did?
 - What lesson can we learn from this?

