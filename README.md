void soma()
{ 
    float valor1, valor2, result; 
    printf("\nDigite o 1 valor: "); 
    scanf ("%f", &valor1); 
    printf("Digite o 2 valor: "); 
    scanf ("%f", &valor2); 
    result = valor1 + valor2; 
    printf("\nResultado: %.2f\n\n ", result); 
}
void subtrai(){ 
    float valor1, valor2, result; 
    printf("\nDigite o 1 valor: "); 
    scanf ("%f", &valor1); 
    printf("Digite o 2 valor: "); 
    scanf ("%f", &valor2);
    result = valor1 - valor2; 
    printf("\nResultado: %.2f\n\n ", result); 
}
void divide(){ 
    float valor1, valor2, result;
    printf("\nDigite o 1 valor: ");
    scanf ("%f", &valor1);
    printf("Digite o 2 valor: ");
    scanf ("%f", &valor2);
    result = valor1 / valor2;
    printf("\nResultado: %.2f\n\n ", result);
    if(valor2 != 0)
            printf("%.2f\n\n", valor1 / valor2);
            else
                printf("Nao existe divisao por 0\n\n");
}
void multiplica()
{
    float valor1, valor2, result;
    printf("\nDigite o 1 valor: ");
    scanf ("%f", &valor1);
    printf("Digite o 2 valor: ");
    scanf ("%f", &valor2);
    result = valor1 * valor2;
    printf("\nResultado: %.2f\n\n ", result);
}
void menu(){ 
    int escolha; 
    printf("Selecione uma operacao matematica:\n"); // msg na tela
    printf("\t1- Adicao\n");
    printf("\t2- Subtracao\n");
    printf("\t3- Divisao\n");
    printf("\t4- Multiplicacao\n");
    printf("Operacao: "); 
    scanf ("%d", &escolha); 

    switch (escolha){ 
        case 1: 
            soma(); 
        break; 

        case 2:
            subtrai();
        break;

        case 3:
            divide();
            
        break;

        case 4:
            multiplica();
            break;


    }
}


int main()
{
    menu(); 
    return 0; 
}
