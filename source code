import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns


df=pd.read_csv("matches.csv")

print(df.head())

#team performance

team_wins = df['winner'].value_counts()
print("\nTeam Wins\n",team_wins)


#player of the match analysis

player_of_match_counts= df['player_of_match'].value_counts()
print("\n Player of the match counts:\n",player_of_match_counts)

#average run score analysis

average_runs_per_match = df['win_by_runs'].mean()
print("\nThe average run scored per match:\n",average_runs_per_match)

# Bar chart of the team wins

plt.figure(figsize=(15,6))
sns.countplot(x='winner', data=df)
plt.title('Number of wins by team')
plt.xlabel('Team')
plt.ylabel('Number of Wins')

#rotate x-axis labels
plt.xticks(rotation=0, fontsize=5)
plt.show()

#Histogram of Runs Scored

plt.figure(figsize=(8,5))
plt.hist(df['win_by_runs'],bins=8)
plt.title('Distribution of runs scored per match')
plt.xlabel('Runs Scored')
plt.ylabel('Frequency')
plt.show()
