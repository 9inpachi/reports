/\_ <img src="https://summerofcode.withgoogle.com/static/favicon/favicon-32x32.png" height="17px" /> Google Summer of Code - <img src="https://www.xwiki.org/xwiki/resources/icons/xwiki/favicon144.png" height="17px" /> **XWiki** \_\

# Interactive Maps Application

A feature rich map application that will allow users to easily create interactive maps within XWiki. Using this application, users can present items of interest on a map in a variety of ways. Data can be associated with each item of interest so users can get more information about the item. Furthermore, using simple to advanced search and filter capabilities, users can easily look for the location they are interested in. Bundled with a lot of customization options to create the map that best suits the user's context.

**Technologies:** Velocity, JavaScript, HTML/CSS, Java

**Mentors:** Stéphane Laurière, Ecaterina Moraru

## Important Links

* [**Extension Page**](https://extensions.xwiki.org/xwiki/bin/view/Extension/InteractiveMapsApplication/)
* [**Project Repository**](https://github.com/xwiki-contrib/application-interactive-maps/)
* [**Daily Progress**](https://github.com/xwiki-contrib/application-interactive-maps/blob/master/PROGRESS.md)
* [**Proposal**](https://drive.google.com/open?id=14qXC7Oy2bPUASfVtSTIsNG1sPcfm5Ikr)
* [**Project Design Page**](https://design.xwiki.org/xwiki/bin/view/Proposal/MapApplication)
* [**Project XWiki Dev Page**](https://dev.xwiki.org/xwiki/bin/view/GoogleSummerOfCode/Map%20application)

## Work

### -  The Community Bonding Period -

During the community bonding period, before getting into the project itself, I started off by fixing issues of other XWiki applications. Since I had no prior knowledge of the **Velocity** template engine, it was a hard road but I eventually got the hang of it once I started writing my own code in it.

### - First Phase -

I started working on the project from 18<sup>th</sup> May, 2019.

During the first week, I started on the project with the my own approach which used preview based map editors to create different kind of maps and developed a lot of generalized functions. At this point, a **simple map** and a **path map** could be created interactively.

**However**, my primary mentor arrived after a week and proposed **a different approach** which was complex but a lot **more flexible** for both simple and advanced users. So I accepted his views and in the second week started working on a **map that used queries** to display data. The general functions I created during the first week helped out until the end.

Moving on, I **implemented points** as a start and used XWiki **Solr Search Query API** to gather those points to display on the map. After that, I implemented **map item and location search** along with **filterable lists** which allowed filtering the data initially gathered.

Then I moved on to improve styling of the map. In the meantime, I got a pull request from my mentor Stephane which included a demo **Map Data Importer**. After accepting the pull request, I **improved the Map Data Importer** by generalizing the import process.

After that I **created UI tests** and the work for the first phase was done.

### - Second Phase -

In the second phase, I started off by implementing **support for custom marker icons**.

Then I **added fullscreen mode** which looked great. From there, I went on to including more options into the map like **map scale, map size etc.** Then I prepared **full documentation** for first release and **made the first public release** of the application.
After that, I **developed a point editor** for easily creating and editing points.

Then I moved **on to shapes** and implemented a mechanism where **shapes could be stored as GeoJSON**.

### - Third Phase -

The third phase was as busy as the prior ones.

As a first step in phase three, I created a **shape editor** which made it easy to create and edit shapes. Then I **implemented styling options** for shapes and points which allowed making the map even more beautiful. I **fixed a lot of bugs** and **made a lot of improvements** during this phase which stabilized the application overall.

I also **implemented indoor structures** where multi-level structures can be presented using shapes and points. I had to **make changes to the leaflet-indoor** library to actually make it work with the latest version of leaflet.

Then I moved on to create a **full fledged map editor** with tools that made creating shapes and points easy.

Finally, I prepared **full documentation** for the **second release** and **released the second version** of the application which marked the end of the my work.

## Remarks

It was a wonderful experience to work with XWiki!

### - The Community -

The XWiki community has always been extremely helpful at every step. I could always get my queries answered on Riot or the mailing list whenever I had a problem.  
I would like to especially thank **Stéphane**, **Ecaterina**, **Thomas**, **Vincent**, **Simon**, **Marius** and **Enygma** for helping me out.

### - Mentors -

Both Stéphane and Ecaterina were extremely helpful throughout the project.  
Stéphane was very detailed in his explanations which always helped me understand things.