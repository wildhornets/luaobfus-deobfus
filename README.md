<h3 align="center">no detailed explanation, find out how to do it by yourself</h3>

`global table.insert` is unused

uses `getfenv();`

uses `setmetatable`

`pcall` is unused

not as safe as msec

`v28` is VM confirmed

```lua
do
  -- globals;
  function init( ... )
    -- decoder loop, var init
  end;
  function VM( ... )
    return function( ... )
      -- ...
    end;
  end;
  return VM(init(), {}, getfenv())(...);
end;
init( encoded, getfenv(), ... )
```
replica of msec vm (almost)

uses idx pointer system

`v81` is opcode

