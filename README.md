# handwriting_questions

I'm working on a task that should read handwritten text, annotate it with suggested changes (or just potential errors), and do some linguistic analysis to provide metric-based feedback. This is intended as a grading _aid_ for student writing.


Questions about reconstructing text and then tokenising it. See the `example_response` json files for actual responses, and csv files for `{googleCloudVisionR}`'s lovely dataframe response.

- Constructing from parsed data: is there are a better strategy than naive `paste`-ing with whitespace, then removing definitely unwanted whitespace (before commas/periods [with exceptions], after opening parentheses etc)
- Reconstructing post-tokenization: is there a better strategy than tokenizing the `description` column then using experience to hard-code exceptions? This seems like a terrible idea, but I can't figure anything better out

Questions about the annotations themselves

- Is there a readily available library that can make annotations to files, leaving the layers on the canvas _separate and still accessible/editable?_
  - applications like [Acrobat](https://www.adobe.com/acrobat.html)/[Drawboard](https://www.drawboard.com/) do it with pdfs
  - pretty much all image editing software does it (but not necessarily to a portable format)
  - all whiteboarding applications seem to be able to do it
  - I think maybe I just don't know _what_ to search for on this one
