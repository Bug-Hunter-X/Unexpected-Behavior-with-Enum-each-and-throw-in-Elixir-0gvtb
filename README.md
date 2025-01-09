# Elixir Enum.each and throw

This example demonstrates a potential issue when using `throw` within an `Enum.each` function in Elixir.  The `throw` statement terminates the `Enum.each` function immediately without properly handling or propagating the exception.  This can lead to unexpected program behavior if not handled within a `try...catch` block. 

The `bug.ex` file demonstrates the problem. The `bugSolution.ex` file provides a corrected version that uses a `try...catch` block to handle the thrown exception gracefully.