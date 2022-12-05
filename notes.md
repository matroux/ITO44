1. We don't see any advantage to rely on 3-rd party services. So we will use our own scripts, and from your side could you just provide the Forms which will POST the html inputs to our scripts.



Not sure of how many forms currently exist, leaving 0.5 hrs as a sensible time estimate.



2. Sorry, but I still not understand your choice. May be we could discuss this directly with the technical staff. For example, taking the page we were discussing last time: content/solutions/cococ33.md (probably should be coco33.md) – why the definition of a custom widget is needed and why the standard approach of Partials can't be used to feed the accordion with content directly from .md files? Firstly, any non-standard approach is harder to understand, and secondly – keeping the content in easily readable .md files would facilitate the maintenance (that was one of our main requirements for the site).



1 - 2 hours would be necessary to create a shortcode which would "wrap" and allow the calling of the already existing partial within the actual markdown content (a technical limitation in Hugo does not allow for partials to be called directly within content), an example of how this looks in action can be seen at https://gohugo.io/content-management/shortcodes/#example-figure-input



3. In order to push your changes, you should "commit" them, then "rebase" your branch on master, then "push" to origin.
But please send us directly as a ZIP file, we will put it on Git.



This does not require an estimate, is more "preferred way to use a tool" kind of matter, but I do understand where this request comes from and agree with it myself.



4. Would it be possible to use a static .css file instead of generating it from .scss? (Your .scss looks simple enough, you have just few variables). Or at least don't generate it each time. Actually, the problem is that .css is generated at each Hugo run (even if nothing is changed in the layout), and the main files are re-generated as well (since the included css file name contains a hash). We will never change the layout, but the content. And at each content modification the .css and all the files of the site will be regenerated (since they all includes the .css). Not very critical, but annoying.



10 minutes to remove the asset hashing from the final CSS output, this solves the main pain point, filename stability (At least from my perspective). An additional 0.5 hours could be allocated to consolidate all the Sass files into a single CSS file if there's an appetite for it.



5. Could you include all the externally referenced CSS and JS into the project?



This is achievable, could be done within 1 hour unless for the typical website project. Under some circumstances it could take longer, that is strongly related to the complexity of the project itself.



6. Please write a comprehensive README file with the description of how to get started to generate the site from Git repository, and the explanation of non-standard (custom) approaches you used to help further understanding.



3 - 5 hours (I am probably over estimating by a large margin), recording topical screencasts to document custom functionality would be the more time efficient way to achieve this. Preparing written documentation would make the estimate to lean to the longer side of the range provided.



7. Please find below a link to download the re-managed PDFs for the publications:
https://www.ito33.com/download/ITO33_Publications.zip
Unlike the Main website page, where the four last articles are displayed with images, could you organize the Publications page as a list of article titles sorted by category, newest to oldest with a short description of each article, without image/thumbnail? It may be something like our current "old" website https://www.ito33.com/publications/technical . Otherwise, we think it would be difficult for a visitor to choose what he wants to read.
Please refer to this page for the short description of each article and the article categories ("Technical Papers", "Fundamental Articles" and "General Publications").



0.5 hours to modify the template and achieve and test the desired output sorting.



Four articles are not in pdf format:
*Technical Papers, "Implied Probability of Bail-In" is a link to Wilmott.com website
*Fundamental Articles:
"contingent claim. Portrait of a philosophy", the link is broken; this article can be removed.
"Plotting the grim reaper’s path", this article is in a page body
*General Publications, "Next Finance", the link is broken; this article can be removed.
