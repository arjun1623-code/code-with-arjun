# code-with-arjun
#include<stdio.h>
#include<math.h>

int main(){
    int start,end,rem,rev=0;
    printf("enter start number :");
    scanf("%d",&start);
    printf("enter the end number :");
    scanf("%d",&end);
    for(int i=start;i<=end;i++){
        int save=i;
        while(i!=0){
            rem=i%10;
            rev=rev*10+rem;
            i=i/10;
        }
        if(save==rev){
            printf("%d",save);
        }
    }
    return 0;
}
