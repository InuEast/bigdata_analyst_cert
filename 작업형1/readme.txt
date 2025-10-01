리드미

# 최대/최소값
df = pd.read_csv('data/corona.csv')

df['ratio'].min() # ratio 최소값
df['ratio'].max() # ratio 최대값

# 그룹화
# 각 국가별로 ratio 열의 최소/최대값 출력
df[['ratio']].groupby(df['country']).min()
df[['ratio']].groupby(df['country']).max()
