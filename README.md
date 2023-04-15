2-) Sequência de Fibonacci, feito com c++, linguagem na qual escolhi por ter um maior conhecimento.
 Usei dois métodos, o qual um usei recursividade e passei por parâmetro um no outro


    void Fibonacci::fibonacciRecursivo(int limite, int ult = 1, int pen = 1) {

    if (limite > 0) {
        int prox = ult + pen;
        cout << prox << " ";
        fibonacciRecursivo(limite - 1, pen, prox);
      }
      
    }

    void Fibonacci::lerDados() {

    int limite;
    cout << "Digite o limite: ";
    cin >> limite;
    fibonacciRecursivo(limite);
    }


3-) Realizei esse exercício de maneira básica com 3 laços de repetição e com um vetor 30, no qual seriam os dias do mês

    float vet[30];
  
    int i, posMenor, posMaior;
    float maior, menor, soma;
    float media;

    for(i=0; i<=29; i++){
    
        cout << "Informe o valor do faturamento do dia " << i+1 << ":" ;
        cin >> vet[i];
        soma += vet[i];
    }
    
    for(i=0; i<29; i++){
        if(vet[i] > maior){
            maior = vet[i];
        }
    }
    menor = vet[0];
    posMenor = vet[0];
    for(i=0; i<29; i++){
        if(vet[i] < menor){
            menor = vet[i];
            posMenor = i;
        }
    }
    media = soma/5;
    
    cout << "\nO maior é: " << maior << endl; 
    cout << "O menor é: " << menor << endl;
    cout << "A média é: " << media << endl;
    
4-) 
   
    float sp= 67836.43, rj = 36678.66, mg = 29229.88, es = 27165.48, outros = 19849.53;
    float total;
    float pRj, pSp, pMg, pEs, pOutros;
    
    
    total = sp + rj + mg + es + outros;
    
    pSp = ((sp/total)*100);
    pRj = ((rj/total)*100);
    pMg = ((mg/total)*100);
    pEs = ((es/total)*100);
    pOutros = ((outros/total)*100);
    
    cout << "São Paulo " <<pSp << "%" << endl;
    cout << "Rio de Janeiro " <<  pRj << "%" << endl;
    cout << "Minas Gerais " << pMg << "%" << endl;
    cout << "Espírito Santo " << pEs << "%" << endl;
    cout << "Outros " << pOutros << "%" << endl;
    
 5-) tentei usar um vetor, para inverrwe uma string
 
    string palavra; 
    int tamanho, i; 

        char c, string[1024];
        
        cout << "Digite uma string: "<< endl;
        cin >> string; 
        
        
        for(i=0; i<tamanho/2; i++)
        {
                c = string[i];
                string[i] = string[tamanho-i-1];
                string[tamanho-i-1] = c;
        }
        cout << "A string invertida -> " << string;
    
    
