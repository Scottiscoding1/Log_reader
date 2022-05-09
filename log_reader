log = open(r"FILE PATH") ##ADD FILE PATH
log_contents = log.read()
user_names = {}

with open(r"FILE PATH") as the_file: ##ADD FILE PATH
    for line in the_file:
        if "Failed password" in line:
            start = line.find("invalid user")
            end = line.find(" from")
            user = line[start+12: end]
            if user not in user_names:
                user_names[user] = 1
            if user in user_names:
                user_names[user] += 1
for user, number in user_names.items():
    print(f"Attackers tried to login using the{user} username {number} times")

log.close()
