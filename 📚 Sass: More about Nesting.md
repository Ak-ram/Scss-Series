this article is also available here: [Sass: More about Nesting📚
](https://dev.to/ak_ram/sass-more-about-nesting-492n)


# Sass: More about Nesting📚
![ssjactc2qsy3romu6er1](https://user-images.githubusercontent.com/69124951/194769461-c03ca4de-fe33-426d-9aa7-e620fdede8bb.png)


We learnt how to nest Scss rules in the [last post](https://dev.to/ak_ram/sass-interpolation-nesting-4d73). Today, we'll go into more depth regarding nesting.

**In this post, we will cover:-**

1. Parent Selector and pseudo-classes
2. Grouping and Nesting CSS Selectors
3. Selector Nest Combinators

Each point will be discussed in depth.

-----

## 1. Parent Selector and pseudo-classes

[Official SASS document](https://sass-lang.com/documentation/style-rules/parent-selector#:~:text=The%20parent%20selector%2C%20%26%20%2C%20is,a%20selector%20before%20the%20parent.) states that

> The parent selector, & , is a special selector invented by Sass that's used in nested selectors to refer to the outer selector

To further understand, consider the example below.

![Example on Parent Selector](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ietox695mfnn9thgdrhh.png)

`&` here works as a reference to the outer selector which is `.main .alert`

---

It may be puzzling to you how such a selector may be helpful, right? Parent selector is most commonly used in:

1.1 _**Suffix classes** context.

Many frameworks, including Bootstrap, have this pattern.

![Example of a parent selector-based suffix class](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/zzfp5v3e933a7cvjc19b.png)


1.2 **_Pseudo classes_** also utilize a parent selector.

![Example on using parent selector with pseudo classes](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ah6hd5ydqzwi9ps15g9x.png)

1.3 also `&` can be used as an argument inside pseudo-selectors functions:

![Example 2 on using parent selector with pseudo classes](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/uxi6xevdqkgd6pxwac5a.png)

## 2. Grouping and Nesting CSS Selectors

We use a comma as a separator when there are many selectors in a list.


![Example on nesting and selector list](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/l7i6bihd1tr8zose93ak.png)

## 3. Selector Nest Combinators (>, +, ~, space)

selector combinators can be placed in many places as shown below:


![where to write selector combinators?](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/33s8w0glve0g9rk9xzz0.png)

Need to read more about selector-nest-combinators? [selector-nest-combinators](https://github.com/stylelint-scss/stylelint-scss/blob/master/src/rules/selector-nest-combinators/README.md)

---

I almost covered everything I know about SCSS nesting; nevertheless, in the following post, we'll talk about a new subject called [placeholder selector](https://sass-lang.com/documentation/style-rules/placeholder-selectors).




























