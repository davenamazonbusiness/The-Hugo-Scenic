---
title: "{{ replace .Name "-" " " | title }}" #Max 70 characters
date: {{ .Date }}
draft: "false" # Set to false to publish
author: ""
description: "Put your description here" #Max 200 characters
summary: "Put your summary here" 
tags: [] 
categories: [] 
## HERO IMAGE ##
# You have to fill the heroImageUrl and the heroImageDescription.
HeroImage: "false" # Change to true if you want to enable hero images
HeroImageUrl: "HERO IMAGE URL"
HeroImageDescription: "HERO IMAGE DESCRIPTION"
HeroImageWidth: ""
HeroImageHeight: ""
## DROPCAP ##
EnableDropcap: "true" #Set to false to disable dropcap
## DISCLAIMER ##
Disclaimer: "false"
DisclaimerTitle: "Disclaimer"
DisclaimerContent: "This is demo content taken from the original article in Wikipedia. It is depicted hare purely for demonstrative reasons."
## STRUCTURED DATA ##
StructuredDataType: "article"
---