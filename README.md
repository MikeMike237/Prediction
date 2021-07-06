def prediction():
    numGames = int(input("How many games to predict? "))
    countries = [["-" for fields in range(4)] for records in range(numGames)]

    for i in range(numGames):
        teamName = input("Enter First Team Name: ")
        countries[i][0] = teamName
        teamGoals = int(input("how many goals has this team scored: "))
        countries[i][1] = teamGoals
        teamName2 = input("Enter second team name: ")
        countries[i][2] = teamName2
        teamGoals2 = int(input("how many goals has this team scored: "))
        countries[i][3] = teamGoals2
        #print(countries)
        if teamGoals > teamGoals2:
            print(teamName,"will be the winner!")
        else:
            print(teamName2,"will be the winner!")



if __name__ == "__main__":
    prediction()
