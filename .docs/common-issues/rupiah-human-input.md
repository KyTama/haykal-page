# Rupiah inputs must accept human notation

A JavaScript regex literal embedded directly in HTML uses one backslash for digit character classes. Escaping that backslash a second time changes the expression's meaning and can silently reject every valid amount.

An HTML number input is also a poor fit when visitors commonly type grouping punctuation or a currency prefix. Use a text input with a numeric input mode, parse one explicit currency grammar, reject non-currency characters and unsafe integers, and format only on blur so caret position stays stable while typing.
