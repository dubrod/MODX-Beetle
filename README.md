# MODX-Beetle
This MODX website theme package is based on the Free theme posted by http://mokaine.com/beetle-free-html/

If you have a MODX Cloud Account you can skip all this setup and email wayne@modx.com to receive a cloud snapshot. 


## Pre-Installation

**Install...**

1. the latest MODX package
2. getResources
3. getPage
4. Collections
5. Archivist
6. Tagger
7. siblingNav
8. Switch
9. pThumb

---

SiblingNav - *core/components/siblingnav/elements/chunks*

**snnext.chunk.html**

```
[[+_isactive:is=`1`:then=`<a href="[[~[[+id]]]]"><span class="label">Next</span><i class="fa fa-chevron-right"></i><span class="sibling-title">[[+menutitle:default=`[[+pagetitle]]`]]</span></a>`:else=``]]
```

**snprev.chunk.html**

```
[[+_isactive:is=`1`:then=`<a href="[[~[[+id]]]]"><i class="fa fa-chevron-left"></i><span class="label">Prev</span><span class="sibling-title">[[+menutitle:default=`[[+pagetitle]]`]]</span></a>`:else=``]]
```

---

## Upload the Transport

1. Extras > Installer
2. "Download Extras" Down Arrow > Upload a package > beetle-1.0-pl.transport.zip
3. Install 

## Configuration

1. Make sure every resource uses the "MX Template"
2. Friendly URLs ON
3. Content > Content Types > HTML = /


### Slider

1. Start a **Collection** for your slides if you want a slider. 
2. You can watch my tutorial video here: https://www.youtube.com/watch?v=rnA5NtaLaYY
3. This theme has some custom Form Customization on this Collection. The xml is available here: https://dl.dropboxusercontent.com/u/4277345/MODX/Form%20Customizations/slider-template-form-customization-set.xml
4. Of course, you can create your own slider component 

### Blog

1. Start a **Collection** for your blog
2. Body Type is **Listing**
3. Body Layout is **Page**
4. Update the Context Setting **blog_id** with your Collection ID

### Archives

1. Start a **Resource** for your Archive template
2. Title "Archive Template"
3. Long Title `[[+arc_month_name]] [[+arc_year]] Archives`
4. Description is shown in the Hero
5. Body Type is **Listing**
6. Body Layout is **Page**
7. Update the Context Setting **archive_id** with your Resource ID

*New Archivist System Setting:*

 - Key: archivist.archive_ids
 - name empty
 - namespace: archivist
 - area lexicon: furls
 - value: 5:arc_  (5 being resource id)

### MENU

1. Start a **Selection** for your MENU
2. Template doesn't matter here
4. Update the Context Setting **menu_id** with your Selection ID

---

 - Resources in **Blog** are "Page" Body Type and Layout, the same for Regular Pages in the Root
 - Update default featured, carousel, and listing Context Settings when you get some content published
 - Watch my 15 minute theme walkthough for more information - https://www.youtube.com/watch?v=0A4JnEOcgUY
 - Visit: http://bettle-theme.clients.modxcloud.com/ to see it in action
 
