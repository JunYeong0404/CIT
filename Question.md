질문 및 답변코딩
====
[김준영]  
질문 : **t는왜 앞에있는 포인터를 가르키나요?

[손정우]  
질문 : 트리가 그래프와 어떤 연관이 있고 그래프에 대한 코딩이 무엇인지 궁금합니다.

[박형민] 
=======
질문 : 링크드 리스트와 밑에 있는 코드에 대해 설명해주세요.

#include <stdio.h>

#include <stdlib.h>

typedef struct list {

 int d;
 
 struct list* p;
 
} LIST;

LIST* root = NULL;

LIST* last = NULL;

void AddList(int a){

 LIST* r = (LIST*)malloc(sizeof(LIST));
 
 r->d = a;
 
 r->p = NULL;
 
 if(root==NULL) root = r;
 
 else           last->p = r;
 
 last = r;
 
}

int main(void){

 AddList(35);
 
 AddList(40);
 
 AddList(45);
 
 while(root){
 
  printf("%d\n", root->d);
  
  root = root->p;
  
 }
}  
[이진욱]
질문 : 더블 포인트에 대한 자세한 설명과 예제가 필요합니다.

[천준영]
질문 : const 함수 와 static 함수의 사용법에 대해 궁금합니다
