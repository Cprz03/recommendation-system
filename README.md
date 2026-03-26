from engine.recommender import recommend_content
from engine.data import content

def main():
    user_preferences = ["programming"]

    recommendations = recommend_content(user_preferences, content)

    print("Recommended Content:\n")
    for item in recommendations:
        print(f"- {item['title']} ({item['category']})")

if __name__ == "__main__":
    main()
