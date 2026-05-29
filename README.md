# SEW_IPOS
Projects written in C.

Used for controlling MOVI-B frequency inverters.

## Bus Positioning

- Enable the drive with DI03
- Use inputs DI04 and DI05 to set the operating mode
- Modes : Jog, Reference, Automatic

> ## Jog mode
> DI04 High, DI05 Low
> 
> Clockwise rotation when DI01 is High.
> 
> Counterclockwise rotation when DI02 is High.

> ## Reference mode
> DI04 Low, DI05 High
>
> Used to set the 0 anchor point to current position.

> ## Automatic mode
> DI04 High, DI05 High
>
> Move the drive to setpoint position.
>
> Start when DI01 is high.

## Cycle positioning

- Set positins 0 and 1
- Move the drive continuously from one position to the other and back
