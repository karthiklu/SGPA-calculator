# SGPA-calculator
name=input("enter a name:")
USN=input("enter a USN:")   
no_of_subjects=int(input("enter  a number of sujects:")) 
total_credits=0
total_earned_credits=0
for i in range(1,no_of_subjects+1): 
          marks=int(input(f"enter a marks scored in subject{i}:"))
          if marks>=90:earned_points=10
          elif 80<=marks<90:earned_points=9         
          elif 70<=marks<80:earned_points=8         
          elif 60<=marks<70:earned_points=7        
          elif 50<=marks<60:earned_points=6      
          elif 40<=marks<50:earned_points=5        
          elif 30<=marks<40:earned_points=4         
          elif 20<=marks<30:earned_points=3       
          elif 10<=marks<20:earned_points=2         
          elif 0<=marks<10:earned_points=1           
          credit=int(input(f"enter a credits of subject{i}:" ))
          total_credits+=credit 
          total_earned_credits+=(earned_points*credit)  
if total_credits>0:          
    print(f"SGPA is:{(total_earned_credits/total_credits):2f}") 
else:print("enter a valid credits")    
  
