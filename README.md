# Reverse__Number
    int reverse(int x) {

    long long rev=0;
    while(x!=0){
        int ld = x % 10; // gives last digit
        rev = rev *10 + ld;
        if(rev ==INT_MAX || rev > INT_MAX){// if else statement came due to some constraints that test cases should pass.
            return 0;
        }  
        if(rev < INT_MIN || rev == INT_MIN){// Because of constraints, rev datatype is long long.
            return 0;
        }
        x =x /10;
    }
    return rev;


    
    }
};
