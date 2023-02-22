def numero1 = 4
def numero2 = 7
pipeline
{
    agent any
    stages
    {
        stage("Escritura")
        {
            steps
            {
                script
                {
                    def calculo1 = numero1*numero2
                    def calculo2 = (numero1+numero2)**2
                    def resultado = "El cálculo de la multiplicacion entre "+numero1+" y "+numero2+" es: "+calculo1+", y el de la suma de las potencias es "+calculo2
                    writeFile (file: "salida.txt", text: resultado)
                }
            }
        }
    }
}
