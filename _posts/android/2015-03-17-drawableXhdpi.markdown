---
layout: post
title:  "按照xhdpi比例格式化获取到的图片"
date:   2015-03-17 14:03:34
categories: android
---
<pre class="brush: java; title: '按照xhdpi比例格式化获取到的图片'">
	private void getXhdpiDrawable(Bitmap imgBitmap){
        DisplayMetrics displayMetrics = MGApp.sApp.getResources().getDisplayMetrics();
        int density = (int)(displayMetrics.densityDpi * displayMetrics.density /2);
        BitmapDrawable imgDrawable= new BitmapDrawable(MGApp.sApp.getResources(),imgBitmap);
        imgDrawable.setTargetDensity(density);
        return imgDrawable;
    }
</pre>


	
<link rel="stylesheet" type="text/css" media="all" href="http://www.alloyteam.com/wp-includes/syntaxhighlighter/styles/shCoreDefault.css" />
<script src="http://apps.bdimg.com/libs/SyntaxHighlighter/3.0.83/scripts/shCore.js"></script>
<script src="http://apps.bdimg.com/libs/SyntaxHighlighter/3.0.83/scripts/shAutoloader.min.js"></script>
<script>function path(){var b=arguments,a=[];for(var c=0;c<b.length;c++){a.push(b[c].replace("@","http://apps.bdimg.com/libs/SyntaxHighlighter/3.0.83/scripts/"))}return a}SyntaxHighlighter.autoloader.apply(null,path("applescript            @shBrushAppleScript.js","actionscript3 as3      @shBrushAS3.js","bash shell             @shBrushBash.js","coldfusion cf          @shBrushColdFusion.js","cpp c                  @shBrushCpp.js","c# c-sharp csharp      @shBrushCSharp.js","css                    @shBrushCss.js","delphi pascal          @shBrushDelphi.js","diff patch pas         @shBrushDiff.js","erl erlang             @shBrushErlang.js","groovy                 @shBrushGroovy.js","java                   @shBrushJava.js","jfx javafx             @shBrushJavaFX.js","js jscript javascript  @shBrushJScript.js","perl pl                @shBrushPerl.js","php                    @shBrushPhp.js","text plain             @shBrushPlain.js","py python              @shBrushPython.js","ruby rails ror rb      @shBrushRuby.js","sass scss              @shBrushSass.js","scala                  @shBrushScala.js","sql                    @shBrushSql.js","vb vbnet               @shBrushVb.js","xml xhtml xslt html    @shBrushXml.js"));SyntaxHighlighter.all();</script>
