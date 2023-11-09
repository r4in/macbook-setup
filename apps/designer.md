# Design Tools

At the end of the day, tools are just tools. But great tools do make the work easier for the craftsman. Feel free to explore what works for your workflow.&#x20;

{% hint style="info" %}
You might want to check the [2022 Design Tools Survey](https://uxtools.co/survey/2022) to see what the industry is using.
{% endhint %}

### **Essentials**

**Adobe Creative Cloud**  🏆

Creative Cloud is basically a launcher for you to download Adobe apps. Installing it via cask is buggy, so I recommend installing it from the web.

[https://creativecloud.adobe.com/apps/download/creative-cloud](https://creativecloud.adobe.com/apps/download/creative-cloud)

You can install whatever you need. What I only need tho is:

* Adobe Photoshop CC 2023
* Adobe Illustrator CC 2023

**SIP**\
A better Color Picker for your Mac.

```
brew install --cask sip
```

### **UI Design**

**Figma** 🏆\
Never had looked back. Currently the best digital design tool out there.

```
brew install --cask figma
```

**Sketch**\
My ex-digital design tool from 2016 - 2018.

```
brew install --cask sketch
```

**Adobe XD**\
For those loyal to the Adobe ecosystem. It can only be installed through the Adobe Creative Cloud launcher. Unfortunately. they will be sun-setting the app. Now, that [Adobe have acquired Figma](https://www.theverge.com/2022/9/17/23357404/adobe-figma-acquisition-20-billion-bet-control-creative-market-antitrust).

{% embed url="https://www.adobe.com/sea/products/xd.html" %}

<details>

<summary><span data-gb-custom-inline data-tag="emoji" data-code="1faa6">🪦</span> Honorable Mentions</summary>

**Abstract**\
Its version control for Sketch

```
brew install --cask abstract
```

I work mostly with Figma - and it has version control baked in already.

**Zeplin**\
Design to developer handoff

```
brew install --cask zeplin
```

My favorite developer handoff tool that integrates nicely with Slack. A bit redundant if you use the Invision + Sketch combo. And very redundant if you're using Figma.

**Craft**\
Excellent plugin for Sketch from Invision

```
brew install --cask craftmanager
```

</details>



### **Digital Whiteboarding**

**FigJam** 🏆

This whiteboarding tool has definitely matured, and using it in Figma saves a lot of subscription costs & app switching.

```
brew install --cask figma
```

**Miro** 🏆\
It's still a top tool for brainstorming & workshopping.

```
brew install --cask miro
```

{% hint style="info" %}
Did you know before Miro, it was previously called RealtimeBoard?
{% endhint %}

<details>

<summary><span data-gb-custom-inline data-tag="emoji" data-code="1faa6">🪦</span> Honorable Mentions</summary>

**Mural**\
Haven't used this in ages. But it's a whiteboarding tool similar to Miro.

</details>



### **Design Systems**

Tools to manage your design systems.

**Figma** 🏆

**Storybook -** [**https://storybook.js.org/**](https://storybook.js.org/?ref=uxtools)

**zeroheight -** [**https://zeroheight.com/**](https://zeroheight.com/)

###

### **User Testing + Recruitment**

Tools used for user testing

**Maze -** [**https://maze.co**](https://maze.co)

**Lyssna (Previously UsabilityHub) -** [**https://www.lyssna.com**](https://www.lyssna.com)

**Usertesting -** [**https://www.usertesting.com**](https://www.usertesting.com)

**UserInterviews** - [https://www.userinterviews.com](https://www.userinterviews.com)



### Research Repository

**Dovetail -** [https://dovetail.com/](https://dovetail.com/insights/)

**Notion**

```
brew install --cask notion
```

**Google Drive**

**Confluence**

### **3D**

**Blender**\
A 3d tool for the pros

```
brew install --cask blender 
```

**Spline**\
A design tool for animating 3D

```
brew install --cask spline 
```



### **Icon Managers**

**Iconset** [🏆](https://emojipedia.org/trophy/)\
A simple icon manager

```
brew install --cask iconset
```

<details>

<summary><span data-gb-custom-inline data-tag="emoji" data-code="1faa6">🪦</span> Honorable Mentions</summary>

**Iconjar** \
An icon Manager

```
brew install --cask iconjar
```

**Nucleo**\
An icon Manager

```
brew install --cask nucleo
```

</details>

{% hint style="warning" %}
I used to be a fan of using icon fonts for design & development because of the ease of use. However, I realized loading a font file is a another http request and might be render-blocking (if you happen to have it on the top fold of the page) Since the dawn of svg, its actually much more lighter\
\
Also, I find myself lately relying more on icon pack libraries in **Figma,** rather than these apps. But it doesn't hurt to have one just incase you need to open it from other apps aside from Figma.
{% endhint %}



###

### **Webfont Generator**

**Fontplop** 🏆\
A Fast, Simple, & Free Open Source Webfont Converter

```
brew install --cask fontplop
```

{% hint style="info" %}
Converting OTF / TTF font files to @font-face used to be a drag and drop thing I usually do at FontSquirrel and other online webfont generators. But having a drag-n-drop native app like this really speeds up my workflow. Previously I used [FontPrep](https://github.com/briangonzalez/fontprep) but was discontinued.
{% endhint %}

###

### Image Optimizers

**Optimage** [🏆](https://emojipedia.org/trophy/)\
Image compression tools

```
brew install --cask optimage
```

**ImageOptim**\
Image compression tools

```
brew install --cask imageoptim
```

{% hint style="warning" %}
Optimizing images should be already baked in your frontend tooling (by running image optimizing npm packages using gulp, react, grunt, ect.) But just incase you need to do it manually, here are some good ones. ImageOptim is free, but the paid alternative Optimage [might be better](https://optimage.app/benchmark). But most frontend tooling, utilizes image compression packages already - you decide.
{% endhint %}

### **Prototyping Tools**

Each of these prototyping tools has its own set of pros and cons. Use each one that fits according to the type of fidelity you need. Most of the time, Figma should be enough.

**ProtoPie** :trophy:

This is [number one](https://uxtools.co/survey/2022/advanced-prototyping) based on the 2022 Design Tools Survey for advaned prototyping.

```
brew install --cask protopie
```

<details>

<summary><span data-gb-custom-inline data-tag="emoji" data-code="1faa6">🪦</span> Deprecated</summary>

**Principle**

```
brew install --cask principle
```

**Flinto**

**Framer**

```
brew install --cask framer
```

**Origami Studio**

```
brew install --cask origami-studio
```



</details>

### Font Managers

**RightFont 8**

```
brew install --cask rightfont
```

**Typeface App**

```
brew install --cask typeface
```

**FontBase**

```
brew install --cask fontbase
```
