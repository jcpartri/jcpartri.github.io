# Extracting Files

&#x2637; [Table of Contents](./../toc.md)

## Lesson Outline

[Extracting Files In The Same Directory](#extracting-files-in-the-same-directory) | [Extracting in Windows / Linux](#extracting-in-windows--linux) | [Extracting in MacOS](#extracting-in-macos) | [Beyond Python](#-beyond-python) | [Challenge](#challenge) | [Summary](#summary)

## Introduction

> &#128214; Luke 24:27 - And beginning with Moses and all the Prophets, he explained to them what was said in all the Scriptures concerning himself.

Extracting or decompressing a zipped file is a little bit like revealing something that is concealed or hidden. The data was compressed and encrypted. It was a mystery before as to what the data meant, but now it is expounded and made plain again. This is what happened on the road to Emmaus. 

On the way to Emmaus, two men were talking about the man Jesus whom they believed to be the promised Messiah. The risen Christ encountered them on the road and after asking them what they were taling about, He Himself explained to them all the things in the Scriptures concerning Himself. Jesus decompressed the scriptures to them. He made the prophesies concerning the Christ plain before them. What a theology lesson that must have been!

In this lesson we are going to learn how to extract the files/projects that we zipped/compressed in the last lesson.

This is going to be super simple. The only thing you need to concern yourself with is **where are you going to extract your files to?**

## Extracting Files in the Same Directory

The most common thing for us to do is to just extract our files into the same folder/directory that our zip files are located in.

### Extracting in Windows / Linux

In Windows / Linux, _right click_ on the .zip file and choose `Extract all`

![right_click](../images/small_right_click.png)

![windows extract](../images/win%20extract%201.png)

Then a dialogue box will appear where you can choose **where** to extract the files/project. For now just choose the same folder where the .zip file is located.

![windows extract 2](../images/win%20extract%202.png)

### Extracting in MacOS

In MacOS is it crazy simple to extract a zip file. Ready? Just double click on the zip file. Viola! Done!

![Uncompressed on Mac](../images/mac%20extract.png)

## Challenge

**Challenge 1:** Can you use what you have learned from these previous lessons, using `mkdir`, `touch`, and other terminal commands to replicate the following sub-file system?

> Note: the .bmp and .py files do not need to contain any data. Making them as empty files is perfectly fine. You are just looking to replicate the structure here.

```console
    main_project/
    ├── images/
    │   ├── alien.bmp
    │   └── ship.bmp
    ├── game.py
    ├── settings.py
    └── scoreboard.py
```

**Challenge 2:** Compress your main_project folder into a .zip file named: `main_project.zip`

**Challenge 3:** Extract your `main_project.zip` file to see if all the contents inside your compressed file were preserved.

## Summary

In this lesson we have learned how to extract files from a compressed .zip file to another folder on your file system.

---

**Projected Lesson Read Time: 5 minutes**

&#8678; Previous Lesson: [Compressing Files](./007_compressing_files.md)

&#8680; Next Lesson: [Chapter Review](./009_review.md)
