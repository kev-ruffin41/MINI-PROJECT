//MINI PROJECT//

#include<stdio.h>
#include<stdlib.h>
#include<conio.h>
#include<string.h>

void main()
{
    int id,pass;
    int c;
    printf("WELCOME TO DZB\n");
    printf("ENTER THE USERID\n");
    scanf("%d",&id);
    if(id==1999)
    {
        printf("ENTER THE PASSWORD\n");
        scanf("%d",&pass);
        if(pass==2000)
        {
            printf("DZB BANK PROVIDES YOU WITH THE FOLLOWING FACILITES\n");
            printf("SELECT THE APPROPRIATE FACILITY YOU WOULD LIKE TO USE\n");
            printf("1.ACCOUNTS\n");
            printf("2.LOANS\n");
            printf("3.INSURANCE\n");
            printf("4.CREDIT AND DEBIT CARD SERVICES\n");
            printf("ENTER THE APPROPRAITE CHOICE FROM ABOVE\n");
            scanf("%d",&c);
            switch(c)
            {
                case 1: printf("MOVE TO COUNTER ACCOUNT 1\n");
                        break;
                case 2: printf("MOVE TO COUNTER LOAN 1\n");
                        break;
                case 3: printf("MOVE TO COUNTER INSURANCE 1\n");
                        break;
                case 4: printf("MOVE TO COUNTER CREDIT/DEBIT SERVICES 1\n");
                        break;
                default: printf("INVALID INPUT\n");
                        break;
            }
        }
        else
        printf("INVALID PASSWORD");
    }
    else
    printf("INVALID USERID");
}

// FORM FILLING FUNCTION//


void formfill()
{
    char v[20],w[20],x[20];
    int y,z;
    int one,pass;

    printf("ENTER THE NAME OF THE MAJOR ACCOUNT HOLDER\n");
    gets(v);
    printf("ENTER THE TYPE OF ACCOUNT YOU WANT TO CREATE\n");
    gets(w);
    printf("ENTER THE ADDRESS OF THE ACCOUNT HOLDER\n");
    gets(x);
    printf("ENTER THE MOBILE NUMBER OF THE ACCOUNT HOLDER\n");
    scanf("%d",&y);
    printf("ENTER THE AMOUNT YOU WOULD LIKE TO DEPOSIT IN THE ACCOUNT\n");
    scanf("%d",&z);

    printf("VERIFY YOUR FINAL DETAILS RELATED TO THE ACCOUNT\n");
    printf("NAME OF THE ACCOUNT HOLDER=%s \n",&v);
    printf("TYPE OF ACCOUNT=%s\n",&w);
    printf("ADDRESS OF THE ACCOUNT HOLDER=%s \n",&x);
    printf("MOBILE NUMBER OF THE ACCOUNT HOLDER=%d \n",&y);
    printf("AMOUNT TO DEPOSIT=%d \n",&z);

    printf("IF ALL THE DETAILS ARE PRECISE ENTER 1");
    scanf("%d",&one);
    if(one=1)
    {
        printf("TO MOVE TO COUNTER ACCOUNT 2 ENTER PASSWORD \n ");
        if(pass==1999)
        printf("COMPLETED");
        else
        printf("INVALID PASSWORD");
    }
}
