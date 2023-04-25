# Laboratorio-ED
Estructura de Datos (25/4/2023 - 1° Semestre)

Árbol Binario de Búsqueda (ABB)
   Crea ABB --> int
   Elimina ABB --> ABB 
   Agrega Número ABB --> int, ABB 
   Busca Número ABB --> int, ABB
   Elimina Número ABB --> int, ABB
   Recorre ABB (En orden) --> ABB

Tipo de estructura
  typedef struct_abb {
    int dato;
    struct_abb* hijoizq;
    struct_abb* hijoder;
  }
  ABB;

Recorre ABB (Ejemplo)
 void recorreABB(ABB* UNABB){
      if (UNABB!=NULL){
         recorreABB(UNABB -> hijoizq);
         printf("%d", UNABB -> Dato);
         recorreABB(UNABB -> hijoder);
      }
 }
