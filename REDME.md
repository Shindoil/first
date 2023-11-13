{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": [],
      "authorship_tag": "ABX9TyNeVp4yhtlw2djrjYFYe+x0",
      "include_colab_link": true
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/Shindoil/first/blob/master/REDME.md\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "- 코랩은 웹브라우저에서 텍스트와 프로그램을 작성할 수 있는 온라인 텍스트 에디터 이다.\n",
        " - 클라우드 기반의 주피터 노트북 개발환경이다.\n",
        " - 코랩은 텍스트를 입력할 수 있는 텍스트 셀과 코드를 입력할 수 있는 코드셀를 제공한다.\n",
        "\n",
        " ### [실행 방법]\n",
        " - Ctrl + Enter : 실행하고 커서가 현재 위치에 그대로 있다.\n",
        " - Alt + Enter : 실행하고 다음 셀을 생성해 준다.\n",
        " - Shift + Enter : 실행하고 이동할 셀이 있으면 이동만하고 이동할 셀이 없으면 새로 셀을 생성한다.\n",
        "\n",
        " ### [ 단축키]\n",
        " - Ctrl + M A  : 코드 셀 위에 삽입\n",
        " - Ctrl + M B  : 코드 셀 아래 삽입\n",
        " - Ctrl + M D  : 셀 삭제\n",
        " - Ctrl + M M  : 마크다운(텍스트)셀로 변경\n",
        " - Ctrl + M Y  : 코드셀로 변경\n",
        " - Ctrl + M Z  : 실행 취소\n",
        " - Ctrl + M H  : 단축키 모음을 보여줌\n",
        "\n",
        "* MAC을 사용하는 경우 Ctrl 대신 Command사용\n",
        "\n",
        "### [ 입력 및 편집 이동]\n",
        " - 입력 -> 편집 이동 : ESC\n",
        " - 편집 -> 입력 이동 : Enter\n",
        "\n",
        "### [제목]\n",
        "제목은 #1 ~ #6가지 형태로 표현할 수 있다.\n",
        "\n",
        "# 제목1\n",
        "## 제목2\n",
        "### 제목3\n",
        "#### 제목4\n",
        "##### 제목5\n",
        "###### 제목6\n",
        "\n",
        "### 구분선\n",
        "-를 세개 이상 쓰면 가로선을 그어 구분영역을 표시할 수 있다.\n",
        "\n",
        "---\n",
        "\n",
        "### 줄바꿈\n",
        "맨 끝에 공백문자 2개 이상(스페이스)을 사용하면 줄바꿈한다.\n",
        "red  \n",
        "green  \n",
        "blue  \n",
        "\n",
        "\n",
        "### 목록\n",
        "순서가 있는 목록과 순서가 없는 목록을 지원한다.\n",
        "1. 리스트1\n",
        "2. 리스트2\n",
        "3. 리스트3\n",
        "\n",
        "- 리스트1\n",
        "- 리스트2\n",
        "- 리스트3\n",
        "  - 리스트3_1\n",
        "  - 리스트3_2"
      ],
      "metadata": {
        "id": "t-wPDBWrm1Nt"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "### 웹주소\n",
        "웹주소를 입력하면 자동으로 하이퍼 링크가 생긴다.  \n",
        "http://www.python.org"
      ],
      "metadata": {
        "id": "-LUkOUONn3CO"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "### 강조\n",
        "***굵게***테스트   \n",
        "___기울기___테스트"
      ],
      "metadata": {
        "id": "RpEqOA69oEU7"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "### 코드블록\n",
        "```python\n",
        "import python\n",
        "def x(self):\n",
        "  return self.x\n",
        "```\n",
        "\n",
        "```java\n",
        "public class Test{\n",
        "  public static void main(String[] args){\n",
        "    System.out.println(\"Hello Java\");\n",
        "  }\n",
        "}\n",
        "```"
      ],
      "metadata": {
        "id": "jW-gz4RLoKpy"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "### 링크\n",
        "[파이썬](http://www.python.org)\n",
        "\n",
        "!를 붙이면 이미지만을 출력할 수 있다.  \n",
        "![python](https://www.python.org/static/img/python-logo.png)  \n",
        "\n",
        "이미지를 클릭했을때 python 사이트로 이동한다.  \n",
        "[![python](https://www.python.org/static/img/python-logo.png)](http://www.python.org)"
      ],
      "metadata": {
        "id": "WI56Cc9qok0z"
      }
    },
    {
      "cell_type": "markdown",
      "source": [],
      "metadata": {
        "id": "6NZdHIsCpkjp"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "def solve_sudoku(board):\n",
        "    empty = find_empty_cell(board)\n",
        "    if not empty:\n",
        "        return True  # 모든 셀이 채워져 있으면 완료\n",
        "\n",
        "    row, col = empty\n",
        "\n",
        "    for num in range(1, 10):\n",
        "        if is_valid(board, num, (row, col)):\n",
        "            board[row][col] = num\n",
        "\n",
        "            if solve_sudoku(board):\n",
        "                return True\n",
        "\n",
        "            board[row][col] = 0\n",
        "\n",
        "    return False\n",
        "\n",
        "def find_empty_cell(board):\n",
        "    for row in range(9):\n",
        "        for col in range(9):\n",
        "            if board[row][col] == 0:\n",
        "                return (row, col)\n",
        "    return None\n",
        "\n",
        "def is_valid(board, num, pos):\n",
        "    row, col = pos\n",
        "\n",
        "    # 행 검사\n",
        "    if num in board[row]:\n",
        "        return False\n",
        "\n",
        "    # 열 검사\n",
        "    if num in [board[i][col] for i in range(9)]:\n",
        "        return False\n",
        "\n",
        "    # 3x3 영역 검사\n",
        "    box_row, box_col = row // 3 * 3, col // 3 * 3\n",
        "    for i in range(box_row, box_row + 3):\n",
        "        for j in range(box_col, box_col + 3):\n",
        "            if board[i][j] == num:\n",
        "                return False\n",
        "\n",
        "    return True\n",
        "\n",
        "# 스도쿠 보드를 입력으로 설정하고 해결\n",
        "sudoku_board = [\n",
        "    [3, 8, 0, 2, 0, 0, 0, 5, 1],\n",
        "    [1, 0, 0, 5, 6, 8, 0, 0, 2],\n",
        "    [0, 5, 0, 1, 0, 3, 8, 9, 0],\n",
        "    [0, 0, 0, 8, 0, 2, 9, 1, 7],\n",
        "    [0, 0, 8, 0, 0, 0, 0, 0, 0],\n",
        "    [0, 0, 0, 0, 3, 0, 0, 0, 8],\n",
        "    [0, 0, 0, 6, 0, 0, 2, 0, 3],\n",
        "    [0, 0, 0, 9, 0, 0, 1, 0, 0],\n",
        "    [5, 0, 0, 3, 1, 0, 0, 0, 9]\n",
        "]\n",
        "\n",
        "solve_sudoku(sudoku_board)\n",
        "\n",
        "for row in sudoku_board:\n",
        "    print(row)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "eN9BJ2s5PVFB",
        "outputId": "f046249b-d9e6-4dfc-8865-9ad4508010ce"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[3, 8, 7, 2, 4, 9, 6, 5, 1]\n",
            "[1, 4, 9, 5, 6, 8, 3, 7, 2]\n",
            "[6, 5, 2, 1, 7, 3, 8, 9, 4]\n",
            "[4, 6, 3, 8, 5, 2, 9, 1, 7]\n",
            "[2, 7, 8, 4, 9, 1, 5, 3, 6]\n",
            "[9, 1, 5, 7, 3, 6, 4, 2, 8]\n",
            "[7, 9, 1, 6, 8, 5, 2, 4, 3]\n",
            "[8, 3, 4, 9, 2, 7, 1, 6, 5]\n",
            "[5, 2, 6, 3, 1, 4, 7, 8, 9]\n"
          ]
        }
      ]
    }
  ]
}