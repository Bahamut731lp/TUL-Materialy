Seznam (angl. **List**) je homogenní, lineární a dynamický [[Abstraktní datový typ|abstraktní datový typ]], který je zobecněním [[FIFO|zásobníku]] a [[LIFO|fronty]]. Narozdíl od nich dovoluje přidávat prvky na libovolné místo seznamu.

>[!tldr]
>- Seznam je zobecněním [[FIFO|zásobníku]] a [[LIFO|fronty]]

Seznamy se dělí podle toho, jak jsou prvky mezi sebou propojeny, na:
- Jednosměrné
- Obousměrné
- Kruhové
   
>[!info] Kruhový seznam
>Kruhový seznam je takový seznam, jehož konec odkazuje na začátek a začátek na konec
>>[!example] Jednosměrný kruhový seznam
>>```mermaid 
>>graph LR 
>>A[Začátek] --> C[1] --> E[2] --> F[...] --> B[Konec] 
>>B --> A
>>```