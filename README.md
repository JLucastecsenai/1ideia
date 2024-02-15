#include <stdio.h>

int main() {
    float a, b, c, d, e, f_moedas, h, i, j, k, l, m, f_notas;
    char g,n,o;

    printf("Voce tem notas? (s/n): ");
    scanf(" %c%c%c", &g,&n,&o);

    switch (g) {
        // Sem notas
        case 'n':
            printf("Quantas moedas de 1 real voce tem?\n ");
            scanf("%f", &a);
            printf("Quantas moedas de 50 centavos voce tem?\n ");
            scanf("%f", &b);
            printf("Quantas moedas de 25 centavos voce tem?\n ");
            scanf("%f", &c);
            printf("Quantas moedas de 10 centavos voce tem?\n ");
            scanf("%f", &d);
            printf("Quantas moedas de 5 centavos voce tem?\n ");
            scanf("%f", &e);
            f_moedas = (a * 1) + (b * 0.5) + (c * 0.25) + (d * 0.1) + (e * 0.05);
            printf("Voce tem R$ %.2f\n", f_moedas);
            break;

        // Com notas
        case 's':
            printf("Quantas notas de 200 reais voce tem?\n ");
            scanf("%f", &f_notas);
            printf("Quantas notas de 100 reais voce tem?\n ");
            scanf("%f", &m);
            printf("Quantas notas de 50 reais voce tem?\n ");
            scanf("%f", &h);
            printf("Quantas notas de 20 reais voce tem?\n ");
            scanf("%f", &i);
            printf("Quantas notas de 10 reais voce tem?\n ");
            scanf("%f", &j);
            printf("Quantas notas de 5 reais voce tem?\n ");
            scanf("%f", &k);
            printf("Quantas notas de 2 reais voce tem?\n ");
            scanf("%f", &l);
            printf("Quantas moedas de 1 real voce tem?\n ");
            scanf("%f", &a);
            printf("Quantas moedas de 50 centavos voce tem?\n ");
            scanf("%f", &b);
            printf("Quantas moedas de 25 centavos voce tem?\n ");
            scanf("%f", &c);
            printf("Quantas moedas de 10 centavos voce tem?\n ");
            scanf("%f", &d);
            printf("Quantas moedas de 5 centavos voce tem?\n ");
            scanf("%f", &e);
            f_moedas = (a * 1) + (b * 0.5) + (c * 0.25) + (d * 0.1) + (e * 0.05);
            f_notas = (f_notas * 200) + (m * 100) + (h * 50) + (i * 20) + (j * 10) + (k * 5) + (l * 2);
            printf("Voce tem R$ %.2f\n", f_moedas + f_notas);
            break;

        default:
            printf("Opcao invalida.\n");
            break;
    }

    return 0;
}
