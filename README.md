rating=float(input("enter the rating of the transformer in volt ampieres or watts:"))
coreloss=float(input("enter the coreloss of the transformer in watts:"))
fLcu_loss=float(input("enter the full load copper loss of the transformer in watts:"))
pf=float(input("enter the power factor or loading of the transformer:"))
k=float(input("enter the load value inserted for the transformer:"))
eff_transf=((k*rating*pf)/((k*rating*pf)+(k*k*fLcu_loss)+coreloss))*100
Kcu_loss=(k*k*fLcu_loss)
ratio=(coreloss/fLcu_loss)
Kmax=pow(ratio,1/2)
print("rating of the transformer at k value of load is:",rating)
print(" rating of the transformer of the transformer at k value of load is:",coreloss)
print("The final efficiency of the transformer at k value of load is:",eff_transf)
print("loading of the transformer at k value of load is:",pf)
print("copper loss of the transformer at k value of load is:",fLcu_loss)
print("The final max efficiency of the transformer at k value of load is:",Kmax)
enter the rating of the transformer in volt ampieres or watts:5000
enter the coreloss of the transformer in watts:100
enter the full load copper loss of the transformer in watts:800
enter the power factor or loading of the transformer:1
enter the load value inserted for the transformer:1
rating of the transformer at k value of load is: 5000.0
 rating of the transformer of the transformer at k value of load is: 100.0
The final efficiency of the transformer at k value of load is: 84.7457627118644
loading of the transformer at k value of load is: 1.0
copper loss of the transformer at k value of load is: 800.0
The final max efficiency of the transformer at k value of load is: 0.3535533905932738
