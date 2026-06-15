# C64 DASM Labels

DASM-compatible C64 memory and KERNAL label mappings.

## Files

- `mapping.asm`: Label constants in DASM syntax (`LABEL = $XXXX`).
- `example-labels.asm`: Short DASM program showing project labels plus code labels.

## Usage

```asm
        processor 6502
        include "mapping.asm"

        org $1000
start:
        lda #$06
        sta BGCOL0
        rts
```
