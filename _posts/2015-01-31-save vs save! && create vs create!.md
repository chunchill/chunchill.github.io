---
layout: post
title:  "save, save!, create, and create!"
date:   2015-01-31 23:22:15
categories:  [Rails]
tags:  [Rails]
---

It turns out that there are two versions of the save and create methods. The variants differ in the way they report errors.

	if order.save 
		# all OK


      order.save!
    rescue RecordInvalid => error
      #validation failed
    end