    float  x, y, z, max, a, b, p, q;
    printf("If the function is of the form f(x) = p*(x^a) - q*(x^b) then enter a and b \n");
    scanf("%f", &a);
    scanf("%f", &b);
    scanf("%f", &p);
    scanf("%f", &q);
    x = (float)0;
    y = (float)0;
    max = y;
    while(x <= (float)40000)
    {
        y = p*pow(x,a) - q*pow(x,b);
        if(max < y)
        {
            max = y;
            z = x;
        }
        x += 0.01;
    }
    printf("The function is maximum at x = %f and the maximum value is %f \n", z, max);
    return 0;
