# ExamJS

> &copy; 2022 Xchuang Corp.
> &copy; BaiG 2022.

### Import

> Download `main.js` or use online version

> Use `<script>` tag to import the code.

```html
<script src="../main.js"></script>
<script src="https://xchuangc.github.io/examjs/main.js"></script>
```

*Download is recommended*

### Create exam widget

> Create a html div tag with id or class.
> Add a script tag with createExamWidget() function.

```html
<div id='exam'></div>
<script>
  createExamWidget('#exam', {/* Question JSON */})
</script>

<div class='exam'></div>
<script>
  createExamWidget('.exam', {/* Question JSON */})
</script>
```

### Question JSON

> Example:

```
{
  title: 'Exam Title',
  question: [
    {
      type: '[(type of input tag)]';
      text: '[Question (Will append to the question) ]',
      prompt : '[Placeholder]',
      questionType : '[FillQ/MCQ]',
      part : '[Part] (Optional)',
      option : ['','',''... (If questionType is MCQ)]
    },
    {},
    {}...
  ],
  partition : [Bool (if true, part is needed)]
}
```
