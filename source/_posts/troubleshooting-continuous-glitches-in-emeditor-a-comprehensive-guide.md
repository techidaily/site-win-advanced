---
title: "Troubleshooting Continuous Glitches in EmEditor: A Comprehensive Guide"
date: 2024-10-24T07:51:09.993Z
updated: 2024-10-29T03:35:10.347Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/a7b1079661cd8a131ebfc4e02675a90ed3f73ee624780bb20b2d8532eb393d21.jpg
---

## Troubleshooting Continuous Glitches in EmEditor: A Comprehensive Guide

Viewing 8 posts - 1 through 8 (of 8 total)

* Author  
Posts
* January 13, 2009 at 11:30 am [#6817](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a9ad075b6df6272e7d2016a18148314b?s=80&d=identicon&r=g)jugaor](https://www.emeditor.com/forums/users/jugaor666/ "View jugaor's profile")  
Participant  
_Hola, amigo Yutaka._  
 EM is a great product, but at your request (“earlier rather than later”) I want to report here several issues (all versions). I numbered’em to facilitate your answers :-D  
 Sorry for my bad English, I’ll try to be as clear as possible.  
 1\. The OR operator with ‘Search Only Word’ got confused if an including word goes first at the expression (two or more):  
 (siempre|sintagma|si) OK, matches ‘siempre’/’sintagma’/’si’  
 (si|siempre|sintagma) BAD, matches ‘si’ but not ‘siempre’/’sintagma’  
 (If this is the expected behavior, please say it at “Regular Expression Syntax” section inside Help)  
 2\. “Find and Replace in Files” operations treat the special chars (‘ñ’, ‘ç’, accented vowels) as word boundaries. For example: “aca” with ‘Search Only Word’ matches the first part of “acañar” or the last parts of “austríaca”, “ilíaca” and so………  
 BUT if “Use Regular Expressions” is enabled too, EM works well (!!!). (F&R at open files never have any problem).  
 3\. Please stop the “Escape sequence” auto triggering in F&R dialog (I already said it in a previous post :-(). Besides the additional click to deactivate it, it always duplicates / and chars at Find Line. A nicer behavior could be remember the last user selection of switches.  
 4\. The dialog “Treat the following characters as alphanumerics” (Customize) is working…? (i.e., it applies to what operations?)  
 If I add any alien char (for example @) EM still treats it as non-letter (using ‘Search Only Word’ or the w operator).  
 5: (Helpfile) Please include two clarifications (for regexp newbies as I… was ;-)):  
 a) The ordinals (º,ª) are always treated as alphanumeric, not word boundaries, so l and w includes’em.  
 b) The “(?” subexpressions allow several strings with I (OR operator), but the lookbehind ones must be lenght fixed.  
 Thank you very much for your time, attention and talent!  
_Saludos desde Perú,_  
 jugaor  
January 13, 2009 at 11:09 pm [#6818](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")  
Keymaster  
I will try to address these issue in the future major version. If v9 beta still has these issues, please let me know. Thank you!  
January 15, 2009 at 6:39 pm [#6821](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")  
Keymaster  
(4.) “Treat the following characters as alphanumeric” option applys only when editing. For instance, when you double-click a word, these characters are treated as a part of the word. However, this setting does not apply to the regular expression w operator nor the Search Only Word option in the Find dialog box. I will clarify the Help description.  
 (5.) I will add a description the lookbehind patterns must be of fixed length .  
 .  
May 19, 2009 at 5:07 am [#7303](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")  
Keymaster  
> jugaor wrote:  
> _Hola, amigo Yutaka._  
> EM is a great product, but at your request (“earlier rather than later”) I want to report here several issues (all versions). I numbered’em to facilitate your answers :-D  
> Sorry for my bad English, I’ll try to be as clear as possible.  
>  
> 1\. The OR operator with ‘Search Only Word’ got confused if an including word goes first at the expression (two or more):  
> (siempre|sintagma|si) OK, matches ‘siempre’/’sintagma’/’si’  
> (si|siempre|sintagma) BAD, matches ‘si’ but not ‘siempre’/’sintagma’  
> (If this is the expected behavior, please say it at “Regular Expression Syntax” section inside Help)  
>  
> 2\. “Find and Replace in Files” operations treat the special chars (‘ñ’, ‘ç’, accented vowels) as word boundaries. For example: “aca” with ‘Search Only Word’ matches the first part of “acañar” or the last parts of “austríaca”, “ilíaca” and so………  
> BUT if “Use Regular Expressions” is enabled too, EM works well (!!!). (F&R at open files never have any problem).  
>  
> 3\. Please stop the “Escape sequence” auto triggering in F&R dialog (I already said it in a previous post :-(). Besides the additional click to deactivate it, it always duplicates / and chars at Find Line. A nicer behavior could be remember the last user selection of switches.  
>  
> 4\. The dialog “Treat the following characters as alphanumerics” (Customize) is working…? (i.e., it applies to what operations?)  
> If I add any alien char (for example @) EM still treats it as non-letter (using ‘Search Only Word’ or the w operator).  
>  
> 5: (Helpfile) Please include two clarifications (for regexp newbies as I… was ;-)):  
> a) The ordinals (º,ª) are always treated as alphanumeric, not word boundaries, so l and w includes’em.  
> b) The “(?” subexpressions allow several strings with I (OR operator), but the lookbehind ones must be lenght fixed.  
>  
> Thank you very much for your time, attention and talent!  
> _Saludos desde Perú,_  
> jugaor  
 “Search Only Word” will not work well with Regular Expressions. Instead, you should use Word Boundaries:  
 The following escape sequences match the boundaries of words:  
 < Matches the start of a word.  
 \> Matches the end of a word.  
 b Matches a word boundary (the start or end of a word).  
 B Matches only when not at a word boundary.  
 I will add thse expressions to the Help.  
 “Treat the following characters as alphanumeric” did not work when searching. This will be fixed in the next alpha version (alpha 19).  
 In order to stop the “Escape sequence” auto trigerring in F&R dialog, you can now uncheck both “Use Selected Text in Find/Replace dialog box” and “Use Word at Cursor in Find/Replace dialog box” in the “Search” tab of the Customize dialog box.  
 Thanks so much for your input!  
May 20, 2009 at 3:14 am [#7305](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a9ad075b6df6272e7d2016a18148314b?s=80&d=identicon&r=g)jugaor](https://www.emeditor.com/forums/users/jugaor666/ "View jugaor's profile")  
Participant  
Thank you for your answers!  
> “Search Only Word” will not work well with Regular Expressions. Instead, you should use Word Boundaries:  
 Please, clarify if this behavior is only at the current version or will be permanent… to begin editing my macros now… :-o  
 Cheers,  
 jugaor  
May 20, 2009 at 5:02 am [#7306](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")  
Keymaster  
> jugaor wrote:  
> Thank you for your answers!  
>  
>> “Search Only Word” will not work well with Regular Expressions. Instead, you should use Word Boundaries:  
>  
> Please, clarify if this behavior is only at the current version or will be permanent… to begin editing my macros now… :-o  
>  
> Cheers,  
> jugaor  
 All versions. The word boundary regular expressions are available both on v8 and v9\. So you shouldn’t use “Search Only Word” checkbox with regular expressions.  
May 20, 2009 at 7:20 am [#7307](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a9ad075b6df6272e7d2016a18148314b?s=80&d=identicon&r=g)jugaor](https://www.emeditor.com/forums/users/jugaor666/ "View jugaor's profile")  
Participant  
OK, thank you!  
 If there are more “hidden” escape sequences ;-) (i.e, not included at the current Help), please, inform here.  
 The additions are always welcome to improve scripting proficiency.  
> In order to stop the “Escape sequence” auto trigerring in F&R dialog, you can now uncheck both “Use Selected Text in Find/Replace dialog box” and “Use Word at Cursor in Find/Replace dialog box” in the “Search” tab of the Customize dialog box.  
 BTW, I didn’t find the first option, only the latest… It changed of dialog box? (v8.05)  
_Un abrazo desde Perú!_  
May 20, 2009 at 9:11 am [#7308](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a9ad075b6df6272e7d2016a18148314b?s=80&d=identicon&r=g)jugaor](https://www.emeditor.com/forums/users/jugaor666/ "View jugaor's profile")  
Participant  
UPDATE:  
 I began to change my scripts and I must say that the results now are more accurate! :-D  
 But, there’s a severe speed penalization, too :-(
 Not the biggest problem in Earth… but If you can optimize this issue, I’ll thank you very much!  
 Thanks again for make this marvelous app better and better with each version!  
_Un abrazo!_
* Author  
Posts

Viewing 8 posts - 1 through 8 (of 8 total)

* You must be logged in to reply to this topic.

<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="autorelaxed"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="1223367746"></ins>

<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="8358498916"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>

<span class="atpl-alsoreadstyle">Also read:</span>
<div><ul>
<li><a href="https://fox-helps.techidaily.com/new-2024-approved-quieting-audio-tracks-for-serenity/"><u>[New] 2024 Approved Quieting Audio Tracks for Serenity</u></a></li>
<li><a href="https://facebook-video-files.techidaily.com/updated-connecting-the-dots-televisions-meet-facebook-lives-for-2024/"><u>[Updated] Connecting the Dots Televisions Meet Facebook Lives for 2024</u></a></li>
<li><a href="https://buynow-help.techidaily.com/a-comprehensive-review-of-twelve-souths-bookbook-v2-accessory-for-your-macbook/"><u>A Comprehensive Review of Twelve South's BookBook V2 Accessory for Your MacBook</u></a></li>
<li><a href="https://win-advanced.techidaily.com/fixen-sie-das-problem-trotz-kriterienerfullung-installiert-sich-windows-11-nicht-hilfe-und-ratschlage/"><u>Fixen Sie Das Problem: Trotz Kriterienerfüllung Installiert Sich Windows 11 Nicht - Hilfe Und Ratschläge</u></a></li>
<li><a href="https://extra-skills.techidaily.com/in-2024-metaversal-motivation-a-curated-list-of-inspiring-quotes/"><u>In 2024, Metaversal Motivation A Curated List of Inspiring Quotes</u></a></li>
<li><a href="https://win-advanced.techidaily.com/leichte-anleitung-zum-wiederherstellen-ihrer-dateien-auf-einer-kaputten-festplatte-eines-computers/"><u>Leichte Anleitung Zum Wiederherstellen Ihrer Dateien Auf Einer Kaputten Festplatte Eines Computers</u></a></li>
<li><a href="https://tech-haven.techidaily.com/sham-botnet-swipes-on-facebook-credentials/"><u>Sham Botnet: Swipes on FACEBOOK Credentials</u></a></li>
<li><a href="https://win-howtos.techidaily.com/step-by-step-solutions-to-overcome-pasting-obstacles-in-windows-11/"><u>Step-by-Step Solutions to Overcome Pasting Obstacles in Windows 11</u></a></li>
<li><a href="https://buynow-reviews.techidaily.com/the-perfect-blend-a-comprehensive-look-at-cost-effective-capability-meets-flagship-flair-in-google-pixel-er/"><u>The Perfect Blend? A Comprehensive Look at Cost-Effective Capability Meets Flagship Flair in Google Pixel Er</u></a></li>
<li><a href="https://win-solutions.techidaily.com/troubleshooting-steps-resolving-constant-stardew-valley-pc-game-crashes/"><u>Troubleshooting Steps: Resolving Constant Stardew Valley PC Game Crashes</u></a></li>
<li><a href="https://win-advanced.techidaily.com/win-11-efi-system-partition-recovery-guide-quick-fix-for-boot-issues/"><u>Win 11 EFI System Partition Recovery Guide - Quick Fix for Boot Issues</u></a></li>
<li><a href="https://win-advanced.techidaily.com/windows-11-file-management-issues-top-tips-for-optimal-performance-and-efficient-data-handling/"><u>Windows 11 File Management Issues : Top Tips for Optimal Performance and Efficient Data Handling</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://bluettide.pxf.io/c/5597632/2141684/17092" target="_top" id="2141684">
  <img src="//a.impactradius-go.com/display-ad/17092-2141684" border="0" alt="https://techidaily.com" width="120" height="90"/>
</a>
<img height="0" width="0" src="https://bluettide.pxf.io/i/5597632/2141684/17092" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

