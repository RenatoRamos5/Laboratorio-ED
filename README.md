# Laboratorio-ED
Estructura de Datos (25/4/2023 - 1° Semestre)

Árbol Binario de Búsqueda (ABB)
   Crea ABB --> *ABB
   Elimina ABB --> *ABB -> int
   Agrega Número ABB --> *ABB, número -> *ABB
   Busca Número ABB --> *ABB, número -> int pos
   Elimina Número ABB --> *ABB, número -> ABB*, int

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
