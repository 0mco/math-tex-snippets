# Math tex snippets
Math tex snippets for UltiSnips

## Getting Started

### Prerequisites
This snippet file is for UltiSnips plugin in Vim, so you need to install UltiSnips in your Vim (if not installing Vim first).

### Installing
To use the snippet file you need to configure UltiSnips, but I didn't try to know how to configure this. I just use vim-snippets plugin to do that for me.

So I recommend you just install vim-snippets plugin like me and copy this file to your vim-snippets directory. It should be '~/.vim/bundle/vim-snippets/UltiSnips/' by default.

## Standards for making rules
* The less, the better (only heavily used typings)
* Convenience
* No confusion
* Do not change users' custom of typing

### Details of standards
When I type LaTeX, I heavily use the arrow keys; and this is a waste of time. So I decided to reduce the use of those keys
I set up a set of snippet to auto-middle for '(', '\[', and '{', etc.
So you just type '()' then the cursor will be in the middle.
When you have finished typing in the parentheses, you can just press '<tab>' to jump out of the parentheses.

## How to use
Only you have done above, you can just start editing your tex file by Vim.
But before that I recommend you have a glance at the snippet file to learn what you can do with this.

### Examples
To type Einstein's field equation
![Einstein's field equation](https://wikimedia.org/api/rest_v1/media/math/render/svg/021a494922172bfe1c9fa4e80d25ac90228d72cf)

We just type
```
eq<tab>\[G_\m<tab> \n<tab><tab> + \L<tab> g_\m<tab> \n<tab><tab> = frac<tab>8\p<tab> G<tab>c^4<tab><tab> T_\m<tab> \n<tab>
```
to get
```
\begin{equation}
	\[ G_{\mu \nu} + \Lambda g_{\mu \nu} = \frac{8\pi G}{c^{4}} T_{\mu \nu} \]
\end{equation}

```
Here I use '\m<tab>' instead of just '\mu' for consistency. At here its convience is not obvious, but when you type '\g<tab>' for '\gamma' or '\e<tab>' for 'epsilon', the convience is clear.
The mappings I used to map these keys to the Greek letters is by the Greek keyboard.
See [GreekKeyboard](https://upload.wikimedia.org/wikipedia/commons/4/48/KB_Greek_polytonic_Unicode.svg) for a complete version.

## Contributing
Any advice to improve is welcome.

## To-do list
* Complete README
* Add some common matrix

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
