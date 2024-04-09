# task-3-
text = input().strip()
pattern = input().strip()
pattern_length = len(pattern)
text_length = len(text)
result = []
for i in range(text_length - pattern_length + 1):
    sub_text = text[i:i + pattern_length]
    if sorted(sub_text) == sorted(pattern):
        result.append(i)
print(result)
