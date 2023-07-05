# Project Euler Solutions

## Problem 1
`$ python -c 'print(sum([x for x in range(1000) if x % 3 == 0 or x % 5 == 0]))'`

## Problem 2
`$ elixir -e "Stream.unfold({1, 2}, fn {a, b} -> {a, {b, a+b}} end) |> Stream.take_while(fn x -> x < 4_000_000 end) |> Stream.reject(fn x -> rem(x, 2) == 1 end) |> Enum.sum()|> IO.inspect()"`
