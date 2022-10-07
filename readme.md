# karasu-utils

**Karasu utils** es un pequeño conjunto de clases para manejar aspectosbásicos del diseño.

## Clases disponibles

### Display

| class  | output  |
| ------------ | ------------ |
| `.inline`  | display: inline  |
| `.block`  | display: block  |
| `.inline-block`  | display: inline-block  |
| `.flex`  | display: flex  |
| `.inline-flex`  | display: inline-flex  |
| `.grid`  | display: grid  |
| `.none`  | display: none  |


### Flexbox

| class  | output  |
| ------------ | ------------ |
| `.jc-start`  | justify-content: flex-start  |
| `.jc-center`  | justify-content: center  |
| `.jc-end`  | justify-content: flex-end  |
| `.jc-around`  | justify-content: space-around  |
| `.jc-between`  | justify-content: space-between  |
| `.jc-evenly`  | justify-content: space-evenly  |
| `.jc-stretch`  | justify-content: stretch  |
| `.jc-revert`  | justify-content: revert  |
| `.ai-start`  | align-items: flex-start  |
| `.ai-center`  | align-items: center  |
| `.ai-end`  | align-items: flex-end  |
| `.ai-baseline`  | align-items: baseline  |
| `.ai-stretch`  | align-items: stretch  |
| `.f-wrap`  | flex-wrap: wrap; |
| `.f-wrap-reverse`  | flex-wrap: wrap-reverse; |
| `.f-nowrap`  | flex-wrap: nowrap; |
| `.f-grow-0`  | flex-grow: 0; |
| `.f-grow-1`  | flex-grow: 1; |
| `.f-row`  | flex-direction: row; |
| `.f-column`  | flex-direction: column; |
| `.f-row-reverse`  | flex-direction: row-reverse; |
| `.f-column-reverse`  | flex-direction: column-reverse; |

### Grid

| class  | output  |
| ------------ | ------------ |
| `.gc-[1~12]`  | --gc: [1~12]  |
| `.gs-[1~12]`  | --gs: [1~12]  |
| `.gap-[1~12]`  | --gap: [1~12]  |

### Gap

| class  | output  |
| ------------ | ------------ |
| `.gap-4`  | gap: 4px  |
| `.gap-8`  | gap: 8px  |
| `.gap-12`  | gap: 12px  |
| `.gap-16`  | gap: 16px  |
| `.gap-20`  | gap: 20px  |
| `.gap-24`  | gap: 24px  |
| `.gap-28`  | gap: 28px  |
| `.gap-32`  | gap: 32px  |
| `.gap-36`  | gap: 36px  |
| `.gap-42`  | gap: 42px  |
| `.gap-48`  | gap: 48px  |

### Margin

| class  | output  |
| ------------ | ------------ |
| `.m4`  | margin: 4px  |
| `.m8`  | margin: 8px  |
| `.m12`  | margin: 12px  |
| `.m16`  | margin: 16px  |
| `.m20`  | margin: 20px  |
| `.m24`  | margin: 24px  |
| `.m28`  | margin: 28px  |
| `.m32`  | margin: 32px  |
| `.m36`  | margin: 36px  |
| `.m42`  | margin: 42px  |
| `.m48`  | margin: 48px  |

Para agregar margen a una dirección en concreto, debemos agregar `-[l|t|r|b]` después de declarar la clase: `m4-l`

### Padding

| class  | output  |
| ------------ | ------------ |
| `.p4`  | padding: 4px  |
| `.p8`  | padding: 8px  |
| `.p12`  | padding: 12px  |
| `.p16`  | padding: 16px  |
| `.p20`  | padding: 20px  |
| `.p24`  | padding: 24px  |
| `.p28`  | padding: 28px  |
| `.p32`  | padding: 32px  |
| `.p36`  | padding: 36px  |
| `.p42`  | padding: 42px  |
| `.p48`  | padding: 48px  |

Igual que hicimos con el *margin*, debemos agregar `-[l|t|r|b]` después de declarar la clase: `.p4-t`

## Breakpoints

Los *breakpoints* o puntos de ruptura están disponible para las clases `flexbox`, `display` y `grid` y se declaran agregando dos puntos seguido del breakpoint especifico: `.jc-start:md`

Hay un total de cinco puntos de ruptura disponible para usar.
| sufijo  | tamaño minimo  | css
| ------------ | ------------ | ------------ |
| `:xs`  | 480px  | `@media screen and (min-width: 480px) { ... }` |
| `:sm`  | 576px  | `@media screen and (min-width: 576px) { ... }` |
| `:md`  | 768px  | `@media screen and (min-width: 768px) { ... }` |
| `:lg`  | 992px  | `@media screen and (min-width: 992px) { ... }` |
| `:xl`  | 1200px  | `@media screen and (min-width: 1200px) { ... }` |

Si necesitas más `breakpoints`, puedes ir a `./src/core/_config.scss` y configurar más si así lo requieres, buscando la variable `$breakpoint`.