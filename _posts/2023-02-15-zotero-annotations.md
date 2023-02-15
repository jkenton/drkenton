---
title: Zotero Annotations as Literature Notes into Obsidian
date: 2023-02-15 06:00:00
layout: post
comments: true
---

<figure>
 <img src="/images/obsidian-logo.png" alt="Obsidian's Logo in PNG format"> <br />
 <img src="/images/zotero-logo.jpeg" alt="Zotero's Logo in JPG format">
 <figcaption>Zotero and Obsidian are good buddies</figcaption>
</figure>

I've gotten quite enamored with the Zettelkasten method after reading Ahrens' book (*How to Take Smart Notes: One Simple Technique to Boost Writing, Learning and Thinking*), and getting to the source material of Niklas Luhmann's original works. [Zettelkasten.de](https://zettelkasten.de/posts/overview/) is a suitable place to get started.

Quickly: I dont know why people insist on suggesting that timestamps are important for zettels. Luhmann never included date information and had a pretty good organizational structure using category codes and alternating numbers and letters to suggest linkages between related notes. The timestamps pushed me off the wagon before.

Also quickly: ideas and insights get into the permanent note collection after starting as "fleeting notes." Most fleeting notes are discarded very quickly, because not every idea is a masterpiece.

Finally: The method suggests that permanent notes are stored and linked. The production of "literature notes" goes along with this process. Literature notes are kept carefully and also stored forever, yet they are not permanent notes. Multiple permanent notes may refer to a given literature note, but I don't believe the literature notes are linked together.

This blog page attempts to describe the process of creating useful literature notes from the Annotations notes made within Zotero. [Check out this resource for more on the mechanics of annotation within Zotero](https://libguides.graduateinstitute.ch/zotero/pdfs). These annotations eventually get into Obsidian, and then I can link to them from the Permanent Notes that are percolating within Obsidian.  [Check out this resource for one user's workflow getting Zotero annotations into Obsidian](https://medium.com/@alexandraphelan/an-academic-workflow-zotero-obsidian-56bf918d51ab).

In my estimation, the usefulness of a reference or a citation is greatly enhanced by being able to see "transcluded" information directly within my Permanent Notes. That is, instead of just creating a reference, or even a link to the literature note, I find it way more useful to see the annotated text directly in the note. [Check out this resource for the use of transclusion in Obsidian](https://jarango.com/2021/09/24/using-transclusion-in-obsidian/). This way, I can make all the comments and summaries that I need right within the Literature Notes and selectively include them within other notes.

Whereas transclusion CAN include the entire note that is being linked, I don't want the entire contents of the note. I only want the "useful" sections of the literature notes to appear in my Permanent Notes. To do this, I borrow the attribute of transclusion that can limitbring in only the contents of a given section, as set off by section headers in the Obsidian document. [Check out Headers and Section syntax here](https://help.obsidian.md/How+to/Format+your+notes#Headers)

With me so far? I hope so...

## Status: 
The Obsidian note that was imported from Zotero is a Literature note. How cool is that?

## Problem: 
Zotero's annotations do not automatically include the # section cues. It may be possible to automatically separate the annotations with section header characters. But they won't automatically have useful and descriptive names, and I don't want EACH highlight or annotation to become its own section. 

## Conditions: 
What I want is to keep together thematically related annotations, and to transclude only the relevant related annotations. Enter Luhmann's method, Obsidian's transclusion function, and a curious mind...

## Onward: 
After creating the Annotation note from a reference document in Zotero, I go into that annotation note and create section headers with meaningful brief descriptors that identify what is in the subsequent annotation.

For example, I might write create a new comment called "## methodology concerns related to secondary data analysis" in the annotation note (see some "Caveats and Pointers" below). 

When an annotations note is fully "section headered," I can import each reference's annotations from Zotero to Obsidian (Using the "Zotero Integration" plugin in Obsidian). Obsidian then creates a Literature note with a name related to the document source in Zotero (AuthornameYearThreeTitleWords is my preferred format). The section headers are in place, placed immediately prior to the relevant passages. For the rest of this description, let's say the imported note was named "Kenton2023ZoteroAnnotationsObsidian."

Cool? Make brief, meaningful section headers in Zotero's Annotation note before importing the annotation into Obsidian.

Now, in a Permanent Note that I am writing in Obsidian, I can transclude only the specific above-mentioned section by typing:

![[Kenton2023ZoteroAnnotationsObsidian]] 

To access a pulldown option of available sections, include a # after the last word of the linked file, like so: 

![[Kenton2023ZoteroAnnotationsObsidian#]]

In that pull down list, there is a section I created, called "Methodology concerns related to secondary data analysis". Select that header. The final link to that transclusion section will become: 

![[Kenton2023ZoteroAnnotationsObsidian#Methodology concerns related to secondary data analysis]]

Lastly, toggle the preview of the note, and see the appropriate section automagically appear. 


## Caveats and Pointers (learned the hard way):

within Zotero's text editor, starting a line with ## will make the following text bold, which is not ideal. So, I usually write the section header at the end of the previous annotation. Then I move the cursor to the space immediately prior to the ##, and hit "Enter" to "trick" Zotero into putting the section header at the beginning of a line. Also, make sure the section header is on its OWN LINE, and that the section header is brief.

Yes, it is possible to do the "section headering" within the imported Obsidian note. Yet, if something happens to the obsidian note (a career in tech support and technology use makes me paranoid and hyperaware of such issues), you can create a new note from Zotero's annotation file. Yet, if you don't make the sections inthe Zotero note, the file imported into Obsidian will need to be "re-section headered". Any links you made in Permanent notes to particular sections will break, unless you are fastidious about renaming the section headers exactly as before. Manually and fastidiously create the section headers in the Zotero Annotation Note.

Related: Make sure to completely annotate the document in Zotero before creating the Annotations note. Otherwise, each time you make new annotations in Zotero and create a new document, the new document will not have any section headers in it. Having to piece together the "Section Headered" portions of multiple files is a real drag.

I choose two ## as my section delimiters merely for my own convenience, and reduced incidence of accidentally making a section where I don't want one in the Zotero Annotation note. 

## Discussion: 
This process has made much more clear to me how the Zettelkasten technique can be useful for making linkages between relatable documents.. 

It also forces me to pre-process the annotation notes in Zotero before importing them into Obsidian as Literature Notes (which is helpful for remembering the contents of the overall reference). Taking the extra time to get that annotation file set up pays multiple dividends down the line. For example, being able to skim the sections when transcluding makes it very easy to get just the right content into the Permanent Note.

I am otherwise a "garbage collector" just highlighting passages and getting the annotations into Obsidian. Because I am unable to remember each context for the contents of the annotations file, it became a source of significant friction to have to re-read, locate the section I wanted, and manually copy-paste the relevent section into a new document. You know, each time I wanted to include something from a Literature Note into a Permanent Note. Yuck. And objectionable, frankly.

Now, the citations are much more accessible and useful and linkable and helpful.

I don't know who else could benefit from this, but if it was you, let me know. My contact info is on the footer of every blog page. Email is great!