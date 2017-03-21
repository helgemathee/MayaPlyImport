import os

env = Environment()

MAYA_DIR = r"C:\Program Files\Autodesk\Maya2017"

env.Append(CPPPATH = os.path.join(MAYA_DIR, 'include'))
env.Append(LIBPATH = os.path.join(MAYA_DIR, 'lib'))
env.Append(LIBS = ['OpenMaya', 'OpenMayaAnim', 'OpenMayaUI', 'OpenMayaRender', 'Foundation'])

sources = Glob('*.cpp')

lib = env.SharedLibrary('MayaPlyImport', sources, SHLIBSUFFIX='.mll', SHLIBPREFIX='')

env.Default(lib)
