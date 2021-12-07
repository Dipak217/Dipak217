from sklearn import tree
def ballpredictor(Weight,Surface):  #(43,Smooth)
    Balls_features = [[35,1],[47,1],[90,0],[48,1],[90,0],[35,1],[92,0],[35,1],[35,1],[35,1],[96,0],[43,1],[110,0],[35,1],[95,0]]
    #1:Rough,2:Smooth  #Features
    Names = [1,1,2,1,2,1,2,1,1,1,2,1,2,1,2]
    #1:Tennis , 2:Cricket   #Labels
    clf = tree.DecisionTreeClassifier()
    clf = clf.fit(Balls_features,Names)
    
    result = clf.predict([[Weight,Surface]]) 
    
    if result == 1:
        print("Your object looks like a Tennis Ball")
        
    if result == 2:
        print("Your object looks like a Cricket Ball")
        
def main():
    print("Enter the Weight of the object: ")
    Weight = input() #43
    
    print("What is the surface type of your object Rough Or Smooth ??")
    Surface = input() #Smooth
    
    if Surface.lower() == "rough":
        Surface = 1
        
    elif Surface.lower() == "smooth":
        Surface = 0
        
    else:
        print("Wrong input")
        exit()
    ballpredictor(Weight,Surface)  #(43, Smooth)
        
main()
