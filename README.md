# quiz10.2

/*
 *  #WSQ14
 *  Created by George.16 on 4/23/15.
 *  Copyright (c) 2015 George.16. All rights reserved.
 *  Main: setprecision(num) << (numero o funcion) <<
 *  #TC1017
 *  Referencia: xxxxxxxxxxxxxxxxxxx
 *
 */
#include <iostream>

using namespace std;

int producto(int x, int p){
    int i = 0, u = 0, z, k;
    int v1[] = {0};
    int v2[] = {0};
    
    for(int i = 1; i <= x; i++){
        cout << "numero para v1" << endl;
        cin >> z;
        
        v1[i] = z;
    }
    
    for(int i = 1; i <= p; i++){
        cout << "numero para v2" << endl;
        cin >> k;
        
        v2[i] = k;
    }


    
    
    do{
        
        u = (v1[i] * v2[i]) + u;
        
        i = i + 1;
        
    }while(i <= x);
    
    
    
    return u;
}


int main(){
    int x, p, u;
    
    cout << "imprime las cantidades para el vector 1" << endl;
    cin >> x;
    
    cout << "imprime las cantidades para el vector 2" << endl;
    
    cin >> p;
    
    if(p == x){
        
        u = producto(x, p);
        
        
    }
    
    else{
        
        cout << "No es posible hacer la multiplicacion ya que no son las mismas cantidades" << endl;
        u = 0;
    }
    
    cout << "El producto punto es igual a " << u << endl;
    
    return 0;
}
