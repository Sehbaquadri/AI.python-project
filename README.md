# AI.python-project
👉 This repository contains my projects and practice work in Python and Artificial intelligence,software development.
{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "\n",
    "# Face Recognition using Principal Component Analysis\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "B4GItm3SaGkm"
   },
   "source": [
    "#### Import Libraries"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 185,
   "metadata": {
    "id": "5V5H-w1KT9Q_"
   },
   "outputs": [],
   "source": [
    "from PIL import Image\n",
    "import numpy as np\n",
    "from numpy import asarray\n",
    "import os\n",
    "import pandas as pd\n",
    "from matplotlib import pyplot as plt\n",
    "from sklearn.preprocessing import StandardScaler\n",
    "from scipy.linalg import eigh\n",
    "from sklearn.metrics import accuracy_score"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "06BxLpbDaLm4"
   },
   "source": [
    "### Import Dataset\n",
    "Assigning labels for the images based on the subdirectories to obtain X(images array) and y (labels).\n",
    "\n",
    "Ensuring that the test data contains atleast one image from each category."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### 1. Loading Dataset and Dividing to Train-Test Splits"
