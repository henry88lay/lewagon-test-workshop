# lewagon-test-workshop

repo and exercises for test workshop

HERE ARE YOUR CHALLENGES!!!

  # Below are the descriptions of each test case as well as the reasoning behind their requirement.

  # 01 - Write a test to verify that the OrangeTree constructor (initialize method) should not take any parameters. We write this test to ensure that there are no permutations on the object class.

  it 'OrangeTree constructor (initialize method) should not take any parameters' do
    initialize_parameters_count = OrangeTree.allocate.method(:initialize).arity
    expect(initialize_parameters_count).to eq 0
  end

  # 02 - Write a test to verify that an instance of the OrangeTree class has a variable with the name "age". As we measure age by number of years, we should also verify that the value of this variable is an integer.

  it 'should have an age' do
    expect(orange_tree).to respond_to :age
    expect(orange_tree.age).to be_a Integer
  end

  # 03 - Write a test to verify that the OrangeTree is 0 years old when created, to ensure that each instance is created at the same baseline. (All instances of the OrangeTree class should be 0 years of age when created.)

  # 04 - Write a test to verify that an instance of the OrangeTree class has a variable with the name "height". As we measure height by number of meters, we should also verify that the value of this variable is an integer.

  # 05 - Write a test to verify that the OrangeTree is 0 meters tall when created, to ensure that each instance is created at the same baseline. (All instances of the OrangeTree class should be 0 meters tall when created.)

  # 06 - Write a test to verify that an instance of the OrangeTree class has a variable with the name "fruits". As we measure the amount of fruits by number , we should also verify that the value of this variable is an integer.

  # 07 - Write a test to verify that the OrangeTree has 0 fruits when created, to ensure that each instance is created at the same baseline. (All instances of the OrangeTree class should be 0 meters tall when created.)

  # 08 - Write a test that would allow you to check a boolean value to determine if the tree is dead or alive. We use a boolean value as it is a simple yes or no test case.

  # 09 - Write a test to verify the existence of the aging method `one_year_passes!`. We write this test to ensure that the method exists and can be called an the instance of the OrangeTree class.

  # 10 - Write a test to verify that after a year passes the age of the orange tree will increase by 1. We write this test to ensure that the tree aging method is working according to the spec. (An orange tree's age will increase by 1 after each time the aging method is called)

  # 11 - Write a test to verify that an orange tree is alive at 50 years of age or below. We write this test to ensure that the tree aging method is working according to the spec. (An orange tree will never die until it is more than 50 years of age)

  # 12 - Write a test to verify that a tree's height does not increase at all after a year passes if its age is 10 or greater. We write this test to ensure that the tree aging method is working according to the spec. (An orange tree does not grow once its age is 10 or more)

  # 13 - Write a test to verify that the tree measures 10 meters when 20 years old, We write this test to ensure that the tree aging method is working according to the spec. (An orange tree does not grow once its age is 10 or more)

  # 14 Write a test to verify that an orange tree can not live if its age is 100 or greater. We write this test to ensure that the tree aging method is working according to the spec. (No tree can live more than 99 years old)

  # 15 Write a test to verify that between 1 years of age to 5 years of age the orange tree produces 0 fruits each year. We write this test to ensure that the method of calculating a trees fruit production is working. (A tree does not grow any fruits each year until it is more than 5 years of age)

  # 16 Write a test to verify that between 6 years of age to 9 years of age the orange tree produces 100 fruits each year. We write this test to ensure that the method of calculating a trees fruit production is working. (A tree grows 100 fruits each year from 6 years of age till 9 years of age)

  # 17 Write a test to verify that between 10 years of age to 14 years of age the orange tree produces 200 fruits each year. We write this test to ensure that the method of calculating a trees fruit production is working. (A tree grows 200 fruits each year from 10 years of age till 14 years of age)

  # 18 Write a test to verify that at 15 years of age the orange tree produces 0 fruits. We write this test to ensure that the method of calculating a trees fruit production is working. (A tree does not grow any fruits when it is 15 years of age)

  # 19 Write a test to verify the existence of the picking method `pick_a_fruit!`. We write this test to ensure that the method exists and can be called an the instance of the OrangeTree class.

  # 20 Write a test to verify that the method `pick_a_fruit!` correctly subtracts 1 fruit from the value of the fruits variable. We write this test to ensure that the method works according to the spec (When `pick_a_fruit!` is called on an instance of the OrangeTree class, the number of fruits it has is reduced by 1)

  # 21 Write a test to verify that the method `pick_a_fruit!` should only subtract 1 fruit from the value fo the fruits variable if that value is greater than 0. We write this test to prevent an instance of the OrangeTree class having a negative number of fruits. (Fruits have to exist to be picked)

  # 22 Write a test to verify that from 50 years old, each successive increase of a trees age, should increase the probability of that tree dying until it has a 100% chance of dying at 100 years old.