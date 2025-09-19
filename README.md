import os

def write_to_file(file_name, content):
    with open(file_name, 'w') as f:
        f.write(content)
    print(f"Đã ghi vào file {file_name}")

def read_from_file(file_name):
    if os.path.exists(file_name):
        with open(file_name, 'r') as f:
            content = f.read()
        print(f"Nội dung file {file_name}:\n{content}")
    else:
        print(f"File {file_name} không tồn tại!")

def main():
    file_name = 'test_github.txt'
    content = "Chào GitHub! Đây là một bài test."
    
    write_to_file(file_name, content)
    read_from_file(file_name)

if __name__ == "__main__":
    main()
