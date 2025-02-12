# Preface {.unnumbered}

This is a side-by-side comparison of the [Polars](https://www.pola.rs/)
and [Pandas](https://pandas.pydata.org/) dataframe libraries,
based on [Modern Pandas](https://tomaugspurger.github.io/posts/modern-8-scaling/) by Tom Augsburger.

(In case you haven't heard, Polars is a very fast and elegant dataframe libary that does the same kinds of things Pandas does.)

The bulk of this book is structured examples of idiomatic Polars and Pandas code, with commentary on the API and performance of both.

For the most part, I argue that Polars is "better" than Pandas, though I do try and make it clear when Polars is lacking a Pandas feature or is otherwise disappointing.

## Who is this for?

This is not a beginner's introduction to data programming, though you certainly don't need to be an expert to read it. If you have some familiarity with any dataframe library, most of the examples should make sense, but if you're familiar with Pandas they'll make even more sense because all the Polars code is accompanied by the equivalent Pandas code.

You don't need to have read *Modern Pandas*, though I of course think it's a great read.

## Why?

AQUI ESTAMOS 
There's this weird phenomenon where people write data programming code as if they hate themselves.
Many of them are academic or quant types who seem to have some complex about being "bad at coding".
Armchair psychology aside, lots of clever folk keep doing [really dumb stuff](https://www.aidancooper.co.uk/pandas-anti-patterns/)
with Pandas, and at some point you have to wonder if the Pandas API is too difficult for its users.

At the very least, articles like [Minimally Sufficient Pandas](https://www.dunderdata.com/blog/minimally-sufficient-pandas)
make a compelling case for Pandas having too much going on.

Having used Pandas a lot, I *think* Polars is more intuitive and does a better job of having One Obvious Way to do stuff. 
It's also much faster at most things, even when you do Pandas the right way.

Hopefully this work shows you how, why and when to prefer Polars.

## Credit

The Pandas examples are mostly lifted from Tom's articles, with some updates for data that's no longer available, and some
code changes to reflect how Pandas is written in 2023. This isn't just me being lazy - I want to draw on Pandas examples that
quite a lot of people are already familiar with.

So credit goes to Tom for the Pandas examples, for most of the data
fetching code and for the general structure of the articles.
Meanwhile the text content and the Polars examples are from me.

## Running the code yourself

You can install the exact packages that the book uses with the [env.yml](https://github.com/kevinheavey/modern-polars/blob/master/env.yml) file:

```shell
mamba env create -f env.yml
```

If you're not using mamba/conda you can install the following package versions and it should work:

```
polars: 1.0.0
pyarrow: 10.0.1
pandas: 2.2.2
numpy: 1.26.4
fsspec: 2024.6.1
matplotlib: 3.8.0
seaborn: 0.13.2
statsmodels: 0.14.2
```

### Data

All the data fetching code is included, but will eventually break as websites change or shut down. The smaller datasets have been checked in [here](https://github.com/kevinheavey/modern-polars/tree/master/data) for posterity.

## Contributing

This book is free and open source, so please do [open an issue](https://github.com/kevinheavey/modern-polars/issues/new) if you notice a problem!
