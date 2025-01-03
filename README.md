This repository demonstrates a subtle bug in Lua related to the `pairs` iterator and nested tables.  When modifying a table during iteration with `pairs`, the iterator's behavior might be unpredictable. This is especially problematic with deeply nested structures. The `bug.lua` file contains the buggy code, and `bugSolution.lua` offers a corrected version. The solution iterates over a copy of the table to prevent unexpected behavior.